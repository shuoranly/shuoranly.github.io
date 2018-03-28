---
layout: post
title:  "super()的使用"
tags: Python
---

# super()的使用介绍
关于super()函数，查看python官方文档的解释如下：<br>
super([type[, object-or-type]])返回一个代理对象，它委托方法给父类或者type的同级类。这对于访问类中被覆盖的继承方法很有用。
除了跳过type本身之外，搜索顺序与getattr()所使用的顺序相同。<br>
通俗点来说就是在类的继承中，如果重定义某个方法，该方法会覆盖父类的同名方法。但有时，我们希望能同时实现父类的功能，
这时我们就需要调用父类的方法了，可通过使用 super 来实现，比如：
