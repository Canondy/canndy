# Github使用指南及优秀开源项目学习

### 1.in关键字  
> in 是用来限定搜索的范围，比如我们通过在名称中搜，在 readme 里搜、在描述里搜

> in:name 在名字中过滤 （发布的仓库名称）<br>
> in:readme 在 Readme 中过滤（说明文档过滤）<br>
> in:description 在简介中过来 <br>

### 2 .stars 、forks
> 我们通过会关系这些项目的流行程度，stars 和 forks 一般是两个比较关系的指标 <br>
> 我们通过 stars 和 forks 条件来过滤 <br>

> 比如我们要过滤，stars > 1000 并且 forks > 1000 的项目，使用 stars:> 和 forks:> <br>
> in:description Laravel  stars:>1000 forks:>1000
 
> 当然你如果需要关系在某个区间过滤，也可以用: start..end <br>
> in:descrption Laravel  stars:1000..2000

### 3.pushed、created 更新日期、创建日期
> 我们在选择一个库的时候，最好选择还在维护的，如果一个库，已经很长时间不更新了，那么我们尽量不要选择，除非已经特别稳定了。我们可以 pushed 来过滤

> in:description 验证码 language:java pushed:>2019-05-01 # 过滤大于 2019-05-01之后提交的 <br>
> in:description 验证码 language:java created:>2019-05-01 # 过滤大于 2019-05-01创建的

### 4.language 编程语言
> 我们也可以根据语言过滤，比如我们搜索一个库的时候，可能只需要对应语言的，就可以通过 language: 进行很快的过滤。比如

> in:description 验证码 language:java 

====================================================================================================

## Github 黑马教程
* SpringCloud、Nacos、Docker、ES、MQ ：https://github.com/LY-1/SpringCloud
* MySQL、Maven、Mybatis、Tomcat、JDBC：https://github.com/Wj-00991314/JavaWebNotes_ItHeiMa
* SpringBoot、MybatisPlus：https://github.com/shuhongfan/SSM_Demo01
* Node.js : https://github.com/tiankainobug/node-study
* html&css：https://github.com/Yanbo-Zhu/HTML5_CSS3_HeiMaPink
* Java基础：https://github.com/tisu97/JAVASE_Notes/tree/master
* Linux: https://github.com/inspire298/Linux
* 解密JVM：https://github.com/2gb0101/Java-JVM
* 看看虚拟机、并发、框架：https://github.com/shuhongfan/Interview_Heima_Demo01
* Netty全套教程（有图解）：https://github.com/shuhongfan/Netty_Demo01
* Netty全套教程（只有代码）： https://github.com/whjpyy/itcast-netty/
* 苍穹外卖（SpringBoot + 微信小程序）：https://github.com/shuhongfan/sky-take-out
* 学成在线（SpringCloudAlibaba + rabbitmq + Vue3）：https://github.com/shuhongfan/xuecheng-plus
* 品达物流 (TMS + APP): https://github.com/shuhongfan/pinda-tms-java
* 黑马头条（Kafka + ES + Hbase）: https://github.com/shuhongfan/heima-leadnew
* 集信达【短信平台】（Docker）：https://github.com/shuhongfan/pd-sms-backend
* 面试 ： https://github.com/shuhongfan/itcast_interview
* 
====================================================================================================

## Java学习优秀作者推荐：

* 掘金~京东云开发者~深入JDK中的Optional（也可看其他博客）：https://juejin.cn/post/7267919941525585977?searchId=20230824020957E74E058FD28BE1826B04
* 面试必备{沉默王二)~~Java面试： https://tobebetterjavaer.com/oo/final.html
* SpringBoot 学习实例   ：https://github.com/ityouknow/spring-boot-examples
* SpringBoot 框架与其它组件结合Jpa、Mybatis、web socket、security、cache等     ：https://github.com/527515025/springBoot
* 技术面试必备基础知识、Leetcode、计算机操作系统、计算机网络、系统设计：https://github.com/CyC2018/CS-Notes


====================================================================================================

## JavaScript前端学习优秀作者推荐：
* 前端学习路径：https://github.com/qianguyihao/Web
* [构建、测试和发现前端代码的最佳场所  代码摸版 可以直接使用](https://codepen.io/)
* [ 12 个 GitHub 上超火的 JavaScript 奇技淫巧项目，找到写 JavaScript 的灵感！](https://github.com/FrontEndGitHub/FrontEndGitHub/issues/14)
* 阮一峰教学文档(JS基础 + 高级)：https://wangdoc.com/
* JavaScript学习资源大全：https://github.com/0e0w/LearnJS
* 20个JavaScript练手项目：https://github.com/bradtraversy/vanillawebprojects
* JavaScript写的2048项目：https://github.com/gd4Ark/2048
* JavaScript50个小项目：https://github.com/bradtraversy/50projects50days
* b站依力学习：https://github.com/orgs/programmer-yili/repositories


## **Vue**
* [Vue3工具大合集](https://vue3js.cn)
* Vue + SpringBoot + MyBatis 音乐网站：https://github.com/Yin-Hongwei/music-website
* Vue仿美团项目（后端使用node.js):https://github.com/zwStar/vue-meituan
* Flutter高仿斗鱼app：https://github.com/yukilzw/dy_flutter

* 张鑫旭的博客：https://www.zhangxinxu.com/
* 淘系前端团队：https://fed.taobao.org/
* Web前端导航：http://www.alloyteam.com/nav/
* 腾讯前端：http://www.alloyteam.com/

* 安卓高仿抖音项目：https://github.com/running-libo/Tiktok
* 安卓高仿网易云项目：https://github.com/aa112901/remusic


====================================================================================================

## Linux 服务器 Vps
* [awesome-selfhosted 自定义服务器 买了服务器不知道要干什么 看他就行了](https://github.com/awesome-selfhosted/awesome-selfhosted)
* [cheat.sh 看看Github 快速查询Linux命令](http://cheat.sh)
* 

====================================================================================================

## Idea插件开发

## [Idea插件破解教程 b站有教程 已收入收藏夹](https://3.jetbra.in)

### IntelliJ-IDEA-Tutorial：https://github.com/judasn/IntelliJ-IDEA-Tutorial/blob/master/plugins-develop.md

#### bilibili搜索  Idea插件开发：
* 京东技术：https://cloud.tencent.com/developer/article/1348741
* 京东云开发者：https://juejin.cn/post/7249380394456596535?searchId=202308240158149CF75832847B567FEE97
* 掘金迈克尔嘿嘿：https://juejin.cn/post/6844904127990857742 （代码好像不全）
* Recording note：https://github.com/AAA-AA/notebook-plugin/tree/master   （配合bilibili视频）
* 跟3是一样的：https://github.com/rongyanjuren/markbook
* 跟 3, 4一样：https://github.com/chengchenrui/mark-book**

====================================================================================================

## 油猴脚本开发 【Tampermonkey, Violentmonkey, Greasemonkey(只有火狐能用), ScriptCat(开源)】

* 油猴开发指南（教程）：https://learn.scriptcat.org/docs/%E7%AE%80%E4%BB%8B/
* 
* Tampermonkey 开源地址(源码)：https://github.com/Tampermonkey/tampermonkey
* Tampermonkey 官网地址：https://www.tampermonkey.net/
* Violentmonkey 开源地址(源码)：https://github.com/violentmonkey/violentmonkey
* Violentmonkey 官网地址(指导、API接口、博客)：https://violentmonkey.github.io/
* ScriptCat 开源地址(源码)：https://github.com/scriptscat/scriptcat
* vite插件，辅助开发（油猴）等脚本引擎的脚本vite-plugin-monkey：https://github.com/lisonge/vite-plugin-monkey/tree/main

====================================================================================================

## 零度解说推荐Github资源：

【看看这个】良心推荐5个免费的容器！不用绑卡、不删数据、不休眠！值得一用 ：https://www.freedidi.com/9313.html

* Cryptomator保护云服务器安全：https://github.com/cryptomator/cryptomator
* Ventoy U盘启动制作工具：https://www.ventoy.net/cn/index.html
* Rocket.Chat 可自由定制的企业级开源通信平台源码：https://github.com/RocketChat/Rocket.Chat
* hackingtool 黑客工具全家桶：https://github.com/Z4nzu/hackingtool
* sniffnet 监控网络流量的工具：https://github.com/GyulyVGC/sniffnet
* Android 获取 Root 权限的工具：https://github.com/topjohnwu/Magisk
* 极简的 uptime 监控工具：https://github.com/louislam/uptime-kuma
* gopeed 一款现代化的下载器（go + drat）：https://github.com/GopeedLab/gopeed
* 开源的问答社区（go + TypeScript）：https://github.com/answerdev/answer
* 开源的文件共享系统（go + HTML）：https://github.com/mtlynch/picoshare
* 开源库存管理系统（Python + JavaScript）：https://github.com/inventree/InvenTree
* python短信轰炸程序（Python + JavaScript）：https://github.com/OpenEthan/SMSBoom
* 开源的服务器监控工具（swift）：https://github.com/Lakr233/Rayon
* 任何视频上的人体抠图：https://github.com/PeterL1n/RobustVideoMatting
* 网站变更检测、监控和通知服务：https://github.com/dgtlmoon/changedetection.io
* 
* 
* Github 上超强的10款开源软件和项目！：https://www.freedidi.com/7587.html
* 推荐10款超级实用的免费开源软件！2023：https://www.freedidi.com/10190.html

====================================================================================================

## Github学习：
* 0.doocs：https://github.com/doocs?q=&type=all&language=java&sort=
* JVM学习：https://doocs.github.io/jvm/   （堆 ，方法区）
* Linux每天命令；https://www.cnblogs.com/peida/archive/2012/12/05/2803591.html
* Java学习及面试指南：https://github.com/Snailclimb/JavaGuide
* JavaGuide(学习与指南)：https://javaguide.cn/
* SpringBlade微服务开发平台: https://github.com/chillzhuang/SpringBlade
* 数据库表结构文档生成器：https://github.com/pingfangushi/screw
* 计算机专业课：https://github.com/SSHeRun/CS-Xmind-Note
* Java小福哥面试：https://github.com/fuzhengwei/CodeGuide
* Java在线考试系统（只是Java代码，还有vue前端代码和各个端系统）：https://github.com/FrontDemon/onlineexam-system-backend
* Java精仿今日头条安卓项目：https://github.com/chaychan/TouTiao

====================================================================================================

## Python
* Python：https://github.com/subbarayudu-j/TheAlgorithms-Python
* python算法：https://github.com/TheAlgorithms/Python
* scikit-learn：Python 中的机器学习：https://github.com/scikit-learn/scikit-learn
* python爬虫教学：https://github.com/wistbean/learn_python3_spider
* 以撸代码的形式学习Python：https://github.com/xianhu/LearnPython
* Python学习：https://github.com/trekhleb/learn-python
* 深度学习：https://github.com/fchollet/deep-learning-with-python-notebooks
* 机器学习：https://github.com/rasbt/python-machine-learning-book
* python-编码/算法问题的解决方案: https://github.com/MTrajK/coding-problems
* 100 多个具有挑战性的 Python 编程练习: https://github.com/zhiwehu/Python-programming-exercises
* 基于项目的教程的精选列表：https://github.com/practical-tutorials/project-based-learning
* 很棒的 Python 框架、库、软件和资源的精选列表: https://github.com/vinta/awesome-python
* Python资源大全中文版: https://github.com/jobbole/awesome-python-cn
* 用 Python 实现的所有算法: https://github.com/TheAlgorithms/Python


* 发卡软件（独角数卡）： https://github.com/assimon/dujiaoka
* 发卡软件（佰阅发卡）：https://github.com/Baiyuetribe/kamiFaka

====================================================================================================

## Swift：
* Swift项目：https://www.jianshu.com/p/757143778db6
* Swift开源项目：https://blog.csdn.net/kyl282889543/article/details/100655409
* AppCoda  Swift and SwiftUI 学习： https://www.appcoda.com/learnswift/swiftui-basics.html
* AppCoda  Swift and UIKit 	 学习； https://www.appcoda.com/learnuikit/get-started.html
* AppCoda  Swift 中级		 学习： https://www.appcoda.com/intermediate-swift-tips/adaptive-ui.html
* Object-C高仿抖音项目：https://github.com/sshiqiao/douyin-ios-objectc

====================================================================================================

## 爬虫：
* 1.路飞学院(樵夫---不包含scrapy)：https://www.bilibili.com/video/BV1PY4y1k7t1?p=76 （ok）
* 2.路飞学院(波波---包含scrapy)：https://www.bilibili.com/video/BV18C4y1a7uk?p=58 （框架开始）
* 3.路飞学院Python爬虫js逆向：https://www.bilibili.com/video/BV1aM4y157oR?spm_id_from=333.999.0.0 （未开始)
* 4.Python爬虫全套+js逆向爬虫  （2和3的合集）：https://www.bilibili.com/video/BV1DR4y1E7uT?spm_id_from=333.999.0.0
* 4.Python爬虫全套课程 （2 + aiphttp异步编程 ： https://www.bilibili.com/video/BV1Yh411o7Sz?spm_id_from=333.999.0.0
* 4.Python爬虫项目（爬取数据+数据整理+数据可视化3小时）
*    (requests + bs4):  https://www.bilibili.com/video/BV1Ry4y1V7PE?spm_id_from=333.999.0.0 （未开始)
* 5.Python爬虫项目（批量获取美女模特照片）（requests + xpath) : https://www.bilibili.com/video/BV1Tu411o7qX?p=3
* 6.Python实战案例合集 爬虫+数据分析+数据可视化展示 （7小时） ：https://www.bilibili.com/video/BV1Fz4y1y7Ct?spm_id_from=333.999.0.0
* 7.爬取微博评论：https://www.bilibili.com/video/BV1dT4y1C7m9/?spm_id_from=333.788
* 8.B站上搜索：python学习者 （100+爬虫案例）
* 9.Python爬虫教程（scrapy框架）：https://www.bilibili.com/video/BV17S4y187B6?spm_id_from=333.999.0.0
* 9.Python爬虫教程（scrapy框架）（和上面的9差不多）：https://www.bilibili.com/video/BV1tt4y1W7zw?spm_id_from=333.999.0.0
 















