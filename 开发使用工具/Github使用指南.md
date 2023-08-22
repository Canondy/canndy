# Github使用指南

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





















