# NVM使用教程(macOS)

>此前电脑上已安装npm和node，不必卸载，不会影响使用

###1使用Homebrew安装nvm
>brew install nvm

注意：安装完成 将以下配置信息添加到 ~/.zshrc 中
>vim ~/.zshrc

>export NVM_DIR="$HOME/.nvm"
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
[ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion

验证nvm安装成功
>nvm -v

###2.是查找本电脑上所有的node版本
>nvm list    或者     nvm ls

>查看已经安装的版本<br>
>nvm list installed 
 
>查看网络可以安装的版本<br>
>nvm list available

>列出所有远程可安装的版本<br>
>nvm ls-remote
###3.安装node
>安装指定版本node <br>
>nvm install  (node版本号）  

>卸载指定的node版本<br>
>nvm uninstall  (node版本号）

>安装最新稳定版 node<br>
>nvm install stable            

>(不推荐使用)安装指定版本，可模糊安装，如：安装v4.4.0，既可nvm install v4.4.0，又可nvm install 4.4 <br>
>nvm install     

###4.切换使用指定的版本
>切换使用指定的node版本<br>
>nvm use (node版本号）

>显示当前node的版本<br>
>nvm current

>为node版本创建别名<br>
>nvm alias (别名名称) (node版本号) 

>删除已定义的别名<br>
>nvm unalias (别名名称)

>在指定版本上重新全局安装依赖库<br>
>nvm reinstall-packages <node版本号>

>显示版本的安装路径<br> 
>nvm which <node版本号或者自定义的别名> 

>查看cache位置<br>
>nvm cache dir 

>安装最新的 npm 版本<br>
>nvm install-latest-npm

###5.不常用
>在指定版本上执行命令<br>
>nvm run <version> [args...] 

>在指定版本上运行交互Shell<br>
>nvm exec <version> [args...] 

>切换镜像源<br>
>nvm mirror <new-mirror> 

>切换node镜像源<br>
>nvm node_mirror <new-mirror> 

>设置代理<br>
>nvm proxy [url] 


###快捷复制模板
><br>
>

><br>
>

><br>
>



