# Python 介绍

本页面主要对 Python 这门语言进行一些简单的介绍，有关互联网上 Python 的介绍也非常多了，读者可以自行搜索就可以了。

## Python 简史
在上个世纪的 80 年代末期（1990 年之前的一年），有关 Python 的历史被改写了。在荷兰的阿姆斯特丹，Centrum Wiskunde & Informatica 大学的 Guido von Rossum 为了让自己的圣诞节有点事情做，不要太无聊了便开始写了 Python 编译器。

1. 1989 年圣诞节：Guido von Rossum 开始写 Python 语言的编译器。
2. 1991年2月：第一个Python编译器（同时也是解释器）诞生，它是用C语言实现的，可以调用 C 语言的库函数。在最早的版本中，Python已经提供了对“类”，“函数”，“异常处理”等构造块的支持，还有对列表、字典等核心数据类型，同时支持以模块为基础来构造应用程序。
3. 1994年1月：Python 1.0正式发布。
4. 2000年10月16日：Python 2.0发布，增加了完整的垃圾回收，提供了对 Unicode的支持。与此同时，Python的整个开发过程更加透明，社区对开发进度的影响逐渐扩大，生态圈开始慢慢形成。
5. 2008年12月3日：Python 3.0发布，它并不完全兼容之前的Python代码，不过因为目前还有不少公司在项目和运维中使用 Python 2.x 版本，所以Python 3.x的很多新特性后来也被移植到Python 2.6/2.7版本中。

目前我们使用的Python 3.7.x 的版本是在2018年发布的，Python的版本号分为三段，形如A.B.C。其中A表示大版本号，一般当整体重写，或出现不向后兼容的改变时，增加A；B表示功能更新，出现新功能时增加B；C表示小的改动（例如：修复了某个Bug），只要有修改就增加C。

如果对Python的历史感兴趣，可以阅读名为自行搜索有关 Python 简史的网络文章。

Python 其实并不是一门新的语言，在 30 多年前就已经诞生了，但随着近年数据处理方面的需求增加，Python 越来越火爆了。

![Python 简史](https://cdn.ossez.com/discourse-uploads/optimized/2X/0/061ee988c05aa2f85c9b028e0438d79a48eb041f_2_276x500.jpeg)

都说尽量不要得罪程序员，搞不好程序员变发飙写一个能够改变世界的东西，看来这个还是有点道理的。

## Python的优缺点

Python的优点很多，简单的可以总结为以下几点。

1. 简单明了，学习曲线低，比很多编程语言都容易上手。
2. 开放源代码，拥有强大的社区和生态圈，尤其是在数据分析和机器学习领域。
3. 解释型语言，天生具有平台可移植性，代码可以工作于不同的操作系统。
4. 对两种主流的编程范式（面向对象编程和函数式编程）都提供了支持。
5. 代码规范程度高，可读性强，适合有代码洁癖和强迫症的人群。

Python的缺点主要集中在以下几点。

1. 执行效率稍低，对执行效率要求高的部分可以由其他语言（如：C、C++）编写。
2. 代码无法加密，但是现在很多公司都不销售卖软件而是销售服务，这个问题会被弱化。
3. 在开发时可以选择的框架太多（如Web框架就有100多个），有选择的地方就有错误。

## 语言对比
因为项目的需要，需要对 Python 进行一些学习，本身长期使用 Java ，所以也难免想使用 Java 来对比下。

因此可能会随时写写自己针对这 2 门语言的小心得。

### 语言类型
Python 是解释型语言。这里需要了解一个叫做 解释型语言 的名词。

在计算机语言体系中，通常有解释型和编译型 2 种语言。用最常见的 Web 开发来说，后端常使用的 Java 就是编译型语言，前端多使用的 JavaScript 就是解释型语言。

针对开发来说，解释型语言是不需要编译器的，但是 解释型语言 需要解释器，比如在网页上写 JavaScript 的代码，你不需要编译后再执行，通常直接刷新页面就可以了。如果你对 Java 代码进行修改后，通常需要再次编译，然后再执行编译结果。

对比 python 和 Java 来说，Python 可以直接写了直接用就行了，和写 JavaScript 差不多。

### 排版布局
Python 语言利用缩进表示语句块的开始和结束（越位规则），而非使用大括号或者某种关键字。增加缩进表示语句块的开始，而减少缩进则表示语句块的结束。根据PEP 8的规定，使用4个空格来表示每级缩进。

使用Tab字符和其它数目的空格虽然都可以被解释器识别，但不符合编码规范，偏向使用Tab字符的程序员可以设置文本编辑器将Tab键转换为4个空格。缩进成为了语法的一部分，并且Python开发者有意让违反了“缩进规则”的程序不能通过解释。

对比 Java 来说，Java 通常是使用 {} 大括号来表达语言结构的，因此可能在最开始使用 Python 的时候有点不适应。

通常使用一些比较好的 IDE 编辑器都能有效的解决这个问题。