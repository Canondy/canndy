# Nginx学习指南

### 1.使用Homebrew安装Nginx

```shell
#使用Homebrew搜索Nginx
brew search nginx                                                                                                                                                                           

#使用Homebrew查看Nginx安装路径，配置文件路径
brew info nginx

#使用Homebrew安装Nginx
brew install nginx

#查看Nginx版本号并验证Nginx是否安装成功
nginx —V

#开启Nginx服务 
brew services start nginx

#重启Nginx服务
brew services restart nginx

#关闭Nginx服务
brew services stop nginx

#文档根目录是 （存放前端项目）
/opt/homebrew/var/www

#Homebrew将Nginx配置文件路径
/opt/homebrew/etc/nginx

#Homebrew将Nginx所有服务存放文件
/opt/homebrew/opt/nginx

#检查配置文件正确性 (检查语法错误,返回成功表示配置可以生效)
nginx -t
nginx -tc <配置文件路径>

#验证配置文件（验证配置文件,更全面地检查可能的问题,可以看到配置文件信息，及mime.types）
nginx -T 


#使用Homebrew更新Nginx
brew upgrade nginx
```

###### 使用Homebrew查看Nginx安装路径，配置文件路径

<img src="/Users/liuhuan/Desktop/截屏2023-08-15 下午6.59.13.png" alt="使用Homebrew查看Nginx安装路径，配置文件路径"  />

###  2.nginx 的配置文件 nginx.conf 包括以下主要部分:

```nginx
nginx中常见的全局块包括:
1. main(全局设置)
2. events(连接设置)
3. http(HTTP设置)
4. server(主机设置)
5. location(URL匹配特定位置的设置)
6. upstream(上游服务器设置)
7. mail(邮件服务器设置)
```

```nginx
nginx 配置文件中的全局块主要用于配置影响 nginx 全局的指令,常见的参数及作用如下:
1. accept_mutex:设置多个工作进程接收连接请求的锁机制,如on或off。
2. accept_mutex_delay:设置接收连接互斥锁的持有时间。单位为毫秒。
3. daemon:设置nginx是否在后台运行。on或off。
4. debug_connection:调试连接函数调用。日志级别为debug。
5. debug_points:启用或禁用调试点。
6. env:设置环境变量,如环境配置文件路径。
7. error_log:设置错误日志文件路径。
8. events:事件模块,处理连接等参数。
9. include:包含外部配置文件。
10. load_module:加载动态模块。
11. lock_file:设置nginx锁文件路径。
12. master_process:启用或禁用master进程。
13. multi_accept:是否允许一个进程接受多个连接。
14. pcre_jit:开启或禁用PCRE JIT功能。
15. pid:设置nginx进程id文件路径。
16. ssl_engine:设置SSL引擎,如OpenSSL。
17. thread_pool:启用线程池。
18. timer_resolution:设置定时器精度。
19. use:设置事件驱动模型,如epoll。
20. user:设置nginx工作进程用户。
21. worker_connections:每个进程允许的最大连接数。
22. worker_cpu_affinity:进程与CPU亲和性。
23. worker_priority:工作进程优先级。
24. worker_processes:工作进程数。
25. worker_rlimit_core: core文件大小。
26. worker_rlimit_nofile:可打开文件数。
27. worker_shutdown_timeout:工作进程退出超时时间。
28. working_directory:设置nginx工作目录。
```

1. ###### 全局块配置影响nginx全局的指令,一般设置运行nginx服务器的用户组,允许生成的worker process数等。

```nginx
user www www; 
worker_processes 4;
pid /var/run/nginx.pid;
```

2. ###### events块影响nginx服务器与用户的网络连接。一般设置每个worker process可以支持的最大连接数。

```nginx
events {
  worker_connections 1024;
}
```

3. ###### http块可以嵌套多个server,配置代理、缓存、日志定义等绝大多数功能和第三方模块的配置。

```nginx
http {
  include /etc/nginx/mime.types;
  server {
    ...
  }

  server {
    ...
  }
}
```

4. ###### server块配置虚拟主机的相关参数,一个http块中可以有多个server块。

```nginx
server {
  listen 80;
  server_name www.example.com;

  location / {
    ...
  }
}
```

5. ###### location块配置匹配的uri位请求进行处理。可以做请求转发、反向代理等功能。

```nginx
location / {
  root /www/site1; 
}

location /images {
  proxy_pass http://image.example.com;
}
```

### 3.反向代理服务器：通过Nginx作为反向代理服务器访问tomcat

```nginx
1.在配置文件nginx.conf  创建同目录文件夹vhosts

2.在nginx.conf的http模块中,需要include引入刚才的配置文件:
http {
  include vhosts/*.conf;
}

3.在vhosts文件夹下创建配置文件 tomcat.conf
server {
  listen 80;                # 监听80端口
  #server_name 127.0.0.1;	#本地测试 有网无网环境都可以
  #使用本配置 
  #无网环境 host需要配置指定本机地址  
      使用域名的方式，访问tomcat
			127.0.0.1 tomcat111.com
			127.0.0.1 tomcat.com
    	可以成功   
  #有网环境 需要申请域名tomcat111.com
  server_name tomcat111.com;	

  location / {

    proxy_set_header X-Forwarded-Host $host;        # 设置请求头Host的值
    proxy_set_header X-Forwarded-Server $host;    # 设置请求头Server的值
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;    # 设置请求头X-Forwarded-For

    #proxy_pass http://127.0.0.1:8080;    # 反向代理到tomcat8080端口
    proxy_pass http://127.0.0.1:8080;    # 反向代理到tomcat8080端口

    proxy_connect_timeout 180;        # proxy 连接超时时间
    proxy_send_timeout 180;            # proxy 发送超时时间
    proxy_read_timeout 180;            # proxy接收超时时间
    proxy_buffer_size 256k;            # 设置代理缓冲区大小
    proxy_buffers 4 256k;            # proxy缓冲区数量及大小
    proxy_busy_buffers_size 256k;        # 高负荷情况下缓冲大小
    proxy_temp_file_write_size 256k;    # 缓冲总大小
  }

}    
    
4.在浏览器中输入    tomcat111.com   就可以访问到tomcat啦
```

### 4.实际应用：使用Nginx反向代理配置---若依Ruoyi-vue前后端分离版

```nginx
server {
    listen       80;
    server_name  localhost; #配置域名
    charset utf-8;

    location / {
      #这个路径是存放dist文件夹内容的位置
      #使用Homebrew安装的Nginx地址是  /opt/homebrew/var/www
      root   /home/ruoyi/projects/ruoyi-ui;	
      try_files $uri $uri/ /index.html;
      index  index.html index.htm;
    }

    location /prod-api/ {
      proxy_set_header Host $http_host;
      proxy_set_header X-Real-IP $remote_addr;
      proxy_set_header REMOTE-HOST $remote_addr;
      proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
      proxy_pass http://localhost:8080/;	#反向代理到后端服务器地址
    }

    error_page   500 502 503 504  /50x.html;
    location = /50x.html {
        root   html;
    }
}
```













