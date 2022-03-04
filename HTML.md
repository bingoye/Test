# HTML

## HTML网页结构

```html
<!DOCTYPE html> 
<html>
 	<head>
        <meta charset="UTF-8">
        <title>页面标题</title>
    </head>
    <body>
        <h1>这是一个标题</h1>
        <p>这是一个段落</p>
    </body>
</html>
```
1. doctype 声明是不区分大小写的，用来告知 Web 浏览器页面使用了哪种 HTML 版本。

在HTML 4.01 中，<!DOCTYPE> 声明需引用 DTD （文档类型声明），因为 HTML 4.01 是基于 SGML（Standard Generalized Markup Language 标准通用标记语言）。

HTML 4.01 规定了三种不同的 <!DOCTYPE> 声明，分别是：Strict、Transitional 和 Frameset。

HTML5 不是基于 SGML，因此不要求引用 DTD。

2. 对于中文网页需要使用 <meta charset="utf-8"> 声明编码，否则会出现乱码。有些浏览器(如 360 浏览器)会设置 GBK 为默认编码，则你需要设置为 <meta charset="gbk">。

目前在大部分浏览器中，直接输出中文会出现中文乱码的情况，这时候需要在头部将字符声明为 UTF-8。

## HTML版本

| 版本      | 发布时间 |
| :-------- | :------- |
| HTML      | 1991     |
| HTML+     | 1993     |
| HTML 2.0  | 1995     |
| HTML 3.2  | 1997     |
| HTML 4.01 | 1999     |
| XHTML 1.0 | 2000     |
| HTML5     | 2012     |
| XHTML5    | 2013     |

### HTML 链接

<a href="https://www.runoob.com">这是一个链接</a>

### HTML 图像

```
loading="lazy" 	延迟请求加载
```

<img loading="lazy" src="logo.png" width="258" height="39" />



<hr>
<!-- 注释 --><br/>

### 文本格式化

<b>这个文本是加粗的</b>

<strong>这个文本是加粗的：定义重要的文本</strong>

<big>这个文本字体放大</big>

<em>这个文本是斜体的：呈现为被强调的文本</em>

<small>这个文本是缩小的</small><sub>下标</sub><sup>上标</sup>

### 预文本格式

<pre>
    定义预格式文本
    	面朝大海	春暖花开
</pre>

### “计算机输出”标签

<code>计算机输出：定义计算机代码</code>

<kbd>键盘输入：定义键盘码</kbd>

<tt>打字机文本</tt>

<samp>计算机代码样本</samp>

<var>计算机变量</var>

<b>注释：</b>这些标签常用于显示计算机/编程代码。

### 地址

<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br> 
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

### 缩写和首字母缩写

<abbr title="etcetera">etc.</abbr>

<acronym title="World Wide Web">WWW</acronym>

<p>在某些浏览器中，当您把鼠标移至缩略词语上时，title 可用于展示表达的完整版本。</p>

### 文字方向

<p>该段落文字从左到右显示。</p>  
<p><bdo dir="rtl">该段落文字从右到左显示。：定义文字方向</bdo></p>  

### 块引用

<p>WWF's goal is to: 
<q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>

### 删除字效果和插入字效果

<p>My favorite color is <del>blue</del> <ins>red</ins>!</p>

### 链接

#### 	图片链接

<p>创建图片链接:
<a href="//www.runoob.com/html/html-tutorial.html">
<img  border="10" src="smiley.gif" alt="HTML 教程" width="32" height="32"></a></p>


<p>无边框的图片链接:
<a href="//www.runoob.com/html/html-tutorial.html">
<img border="0" src="smiley.gif" alt="HTML 教程" width="32" height="32"></a></p>

#### 	书签链接

```HTML
<p>
<a href="#C4">查看章节 4</a>
</p>

<h2>章节 1</h2>
<p>这边显示该章节的内容……</p>

<h2>章节 2</h2>
<p>这边显示该章节的内容……</p>

<h2>章节 3</h2>
<p>这边显示该章节的内容……</p>

<h2><a id="C4">章节 4</a></h2>
<p>这边显示该章节的内容……</p>

<h2>章节 5</h2>
<p>这边显示该章节的内容……</p>
```

#### 	跳出框架

<p>跳出框架?</p> 
<a href="//www.runoob.com/" target="_top">点击这里!</a> 

#### 	创建电子邮箱链接

<p>
这是一个电子邮件链接：
<a href="mailto:someone@example.com?Subject=Hello%20again" target="_top">
发送邮件</a>
</p>

<p>
<b>注意:</b> 单词之间空格使用 %20 代替，以确保浏览器可以正常显示文本。
</p>

<p>
这是另一个电子邮件链接：
<a href="mailto:someone@example.com?cc=someoneelse@example.com&bcc=andsomeoneelse@example.com&subject=Summer%20Party&body=You%20are%20invited%20to%20a%20big%20summer%20party!" target="_top">发送邮件!</a>
</p>