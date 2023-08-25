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

======================================================================================================

### Github学习 | Swift | 爬虫 | Linux学习 <br>
#### Github学习：
  * 0.doocs：https://github.com/doocs?q=&type=all&language=java&sort=
  *    JVM学习：https://doocs.github.io/jvm/   （堆 ，方法区）
  *    Linux每天命令；https://www.cnblogs.com/peida/archive/2012/12/05/2803591.html
  * 1.Java学习及面试指南：https://github.com/Snailclimb/JavaGuide
  * 2.20个js练手项目：https://github.com/bradtraversy/vanillawebprojects
  * 3.js写的2048项目：https://github.com/gd4Ark/2048
  * 4.js50个小项目：https://github.com/bradtraversy/50projects50days
  * 5.Vue + SpringBoot + MyBatis 音乐网站：https://github.com/Yin-Hongwei/music-website
  * 6.SpringBlade微服务开发平台: https://github.com/chillzhuang/SpringBlade
  * 7.数据库表结构文档生成器：https://github.com/pingfangushi/screw
  * 8.计算机专业课：https://github.com/SSHeRun/CS-Xmind-Note
  * 9.b站依力学习：https://github.com/orgs/programmer-yili/repositories
  * 10.Python：https://github.com/subbarayudu-j/TheAlgorithms-Python
  * 11.python算法：https://github.com/TheAlgorithms/Python
  * 12.scikit-learn：Python 中的机器学习：https://github.com/scikit-learn/scikit-learn
  * 13.python爬虫教学：https://github.com/wistbean/learn_python3_spider
  * 14.以撸代码的形式学习Python：https://github.com/xianhu/LearnPython
  * 15.Python学习：https://github.com/trekhleb/learn-python
  * 16.深度学习：https://github.com/fchollet/deep-learning-with-python-notebooks
  * 17.机器学习：https://github.com/rasbt/python-machine-learning-book
  * 18.python-编码/算法问题的解决方案: https://github.com/MTrajK/coding-problems
  * 19.100 多个具有挑战性的 Python 编程练习: https://github.com/zhiwehu/Python-programming-exercises
  * 20.基于项目的教程的精选列表：https://github.com/practical-tutorials/project-based-learning
  * 21.很棒的 Python 框架、库、软件和资源的精选列表: https://github.com/vinta/awesome-python
  * 22.Python资源大全中文版: https://github.com/jobbole/awesome-python-cn
  * 23.用 Python 实现的所有算法: https://github.com/TheAlgorithms/Python
  * 24.Java小福哥面试：https://github.com/fuzhengwei/CodeGuide
  * 25.Java在线考试系统（只是Java代码，还有vue前端代码和各个端系统）：https://github.com/FrontDemon/onlineexam-system-backend
  * 26.Java精仿今日头条安卓项目：https://github.com/chaychan/TouTiao
  * 27.Object-C高仿抖音项目：https://github.com/sshiqiao/douyin-ios-objectc
  * 28.安卓高仿抖音项目：https://github.com/running-libo/Tiktok
  * 29.安卓高仿网易云项目：https://github.com/aa112901/remusic
  * 30.Vue仿美团项目（后端使用node.js):https://github.com/zwStar/vue-meituan
  * 31.Flutter高仿斗鱼app：https://github.com/yukilzw/dy_flutter
  * 32.前端学习路径：https://github.com/qianguyihao/Web
  * 33.JavaGuide(学习与指南)：https://javaguide.cn/
  * 34.发卡软件（独角数卡）： https://github.com/assimon/dujiaoka
  * 35.发卡软件（佰阅发卡）：https://github.com/Baiyuetribe/kamiFaka

#### Swift：
  * 1.Swift项目：https://www.jianshu.com/p/757143778db6
  * 2.sSwift开源项目：https://blog.csdn.net/kyl282889543/article/details/100655409
  * 3.AppCoda  Swift and SwiftUI 学习： https://www.appcoda.com/learnswift/swiftui-basics.html
  * 4.AppCoda  Swift and UIKit 	 学习； https://www.appcoda.com/learnuikit/get-started.html
  * 5.AppCoda  Swift 中级		 学习： https://www.appcoda.com/intermediate-swift-tips/adaptive-ui.html

#### 爬虫：
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
 















