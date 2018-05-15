---
title: html知识总结
date: 2018-05-15 16:06:15
tags:
---

### HungryWalley笔记
 ---

###### 1.网址
https://explainshell.com/    解释linux命令 <br/>
www.namesilo.com             便宜的域名    <br/>
www.500d.me                  好看的简历    <br/>
dribbble.com                 顶级设计师聚集




###### 2.html

- a标签里面的href究竟能写什么？
```html
<a href= ""></a>
```
例如想要跳转到qq.com 就不可以写 href="qq.com" ，不然浏览器会以为这是相对路径（文件），要写成 http://qq.com, http协议要声明http，//表示当前协议，如果当前是windows文件协议，那么只写//的话就只是打开【文件树】

- 点击以后什么也不做的a标签
```
<a href= "javascript:void(0);"></a>
```
或者

```
<a href= "javascript: ;"></a>
```

- a标签和form标签的区别

    a标签发起的是get请求，form标签发起的是get,post请求<br/>
    form 标签里面有一个 button 元素，button 的 type 属性为空，也可以提交表单

- iframe 属性了解一下

    https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe

- 根据 HTML 规范 ，table的子元素可以是

    thead
    tbody
    tfoot
    colgroup




###### 3.css

下面哪些元素的默认 display 为 block
    ```
    div ul h1
    ```

body 标签的默认 margin 是多少像素

    8

如何用 meta 声明当前页面的 charset？

    <meta charset="utf-8">
    <meta http-equiv="content-type" content="text/html; charset=utf-8" >
    第二种写法是为了不久后端开发忘了设置 http 的 content-type


CSS 里，可替换元素（replaced element）的展现不是由CSS来控制的。这些元素是一类 外观渲染独立于CSS的 外部对象。 典型的可替换元素有 img、 object、 video 和 表单元素，如textarea、 input 某些元素只在一些特殊情况下表现为可替换元素，例如 audio 和 canvas 。 通过 CSS content 属性来插入的对象 被称作 匿名可替换元素（anonymous replaced elements）。
CSS在某些情况下会对可替换元素做特殊处理，比如计算外边距和一些auto值。
需要注意的是，一部分（并非全部）可替换元素，本身具有尺寸和基线（baseline），会被像vertical-align之类的一些 CSS 属性用到。

###### 4.javascript

1. noscript 标签

>在有些浏览器禁用脚本，或者脚本未被支持，这时候，则noscript里面的脚本定义了替代的内容（生效）

https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/noscript
