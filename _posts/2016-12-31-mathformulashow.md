---
layout: post
title: "在Blog中显示Markdown中数学公式"
date: 2016-12-31 
description: "解决数学公式在Blog中无法显示的问题"
tag: Markdown  

---

在我们写博客的时候，有时就会遇到写出的数学公式在前端无法显示。    
例如下面这一条数学公式：   
$f(x,y,z)=3y2z\left(3+\frac{7x+5}{1+y^2}\right) $  
可以看出并没有显示出公式。  
当然解决的方法有很多，比如将数学公式截图成图片插入到Markdown中。但是这种方法有一个很严重的缺点就是数学公式非常模糊。   
这次我介绍的一种解决方式是使用mathjax的方式对数学公式进行展示。而且使用MathJax的方式非常简单，只需要在Markdown文件中插入一条脚本代码即可。  
### 脚本代码

```html
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
```


将该段代码插入到自己写的MarkDown中，并将Markdown放在自己博客目录下。在该篇博文加载的时候，就会调用该条脚本，执行脚本，就会处理博文中的数学公式。   
### 注意事项

MathJax能够处理LaTeX方式的数学公式，在写数学公式的时候最好使用Latex   

### 效果展示

<center> $$ f(x,y,z)=3y2z\left(3+\frac{7x+5}{1+y^2}\right) $$  </center>


