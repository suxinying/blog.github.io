---
title: JavaScript权威指南第13章Web浏览器中的JavaScript
date: 2020-04-10 22:19:48
tags: JavaScript权威指南
categories: JavaScript
---

[TOC]

### 13.2 在HTML中嵌入JavaScript

- 内联，放置在`<script>`和`</script>`标签对之间
- 放置在由`<script>`标签的`src`属性指向外部文件中
- 放置在HTML时间处理中，该事件处理程序由`onclick`或`onmouseover`这样的HTML属性值制定
- 放置在一个URL中，这个URL使用特殊的`javascript:`协议

#### 外部文件中的脚本

##### 优点

- 可以把大块JavaScript代码从HTML文件中删除，这有助于保持内容和行为的分离，从而简化HTML开发
- 如果多个WEB页面使用共同的JavaScript代码，用`src`属性可以让你只管理一份代码
- 如果一个JavaScript代码文件由多个页面共享，就只需要下载它一次，随后的页面能够通过浏览器缓存检索它
- 由于`src`属性可以是任意的URL，因此来自一个Web服务器的JavaScript程序或Web页面可以使用另一个Web服务输出的代码。