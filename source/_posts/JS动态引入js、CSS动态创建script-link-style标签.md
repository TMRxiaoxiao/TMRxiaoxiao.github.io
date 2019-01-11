---
title: JS动态引入js、CSS动态创建script/link/style标签
date: 2019-01-11 14:03:15
tags: 技术
---

### 一，动态创建link方式

> 代码如下

```js
function addCssByLink(url){ 
    var doc=document; 
    var link=doc.createElement("link"); 
    link.setAttribute("rel", "stylesheet"); 
    link.setAttribute("type", "text/css"); 
    link.setAttribute("href", url); 
   
    var heads = doc.getElementsByTagName("head"); 
    if(heads.length) 
        heads[0].appendChild(link); 
    else 
        doc.documentElement.appendChild(link); 
} 
```

<!--more-->

### 二，动态创建style方式

> 但是,这样的话,需要加载整个css文件,但是那样有可能浪费一个http请求并占用一个服务器请求数,并等待上一段下载时间,所以,Firebug Lite采取的是将css代码写在js中,然后动态创建style标签的方法,正如下面所示

```js
function addCssByStyle(cssString){ 
    var doc=document; 
    var style=doc.createElement("style"); 
    style.setAttribute("type", "text/css"); 
   
    if(style.styleSheet){// IE 
        style.styleSheet.cssText = cssString; 
    } else {// w3c 
        var cssText = doc.createTextNode(cssString); 
        style.appendChild(cssText); 
    } 
   
    var heads = doc.getElementsByTagName("head"); 
    if(heads.length) 
        heads[0].appendChild(style); 
    else 
        doc.documentElement.appendChild(style); 
} 
```

> 这样的话,如果是较少的代码,可以比较方便的实现到动态加载css的效果,但是如果为了方便维护和管理,并没有等待时间限制,使用link方式更加合适

### 三,动态创建script方式

> 代码如下

```js
var script=document.createElement("script"); 
script.setAttribute("type", "text/javascript"); 
script.setAttribute("src", "JustWalking.js"); 
var heads = document.getElementsByTagName("head"); 
if(heads.length) 
    heads[0].appendChild(script); 
else 
    document.documentElement.appendChild(script); 
```

> 这种方式在IE内核的浏览器中支持，但是在google、360极速、firefox下却不行

### 四，打印引入style方式

```js
document.write("<link rel=\"stylesheet\" href=\"uild/style.css\" type=\"text/css\" media=\"screen\"/>"); 
```

### 五，打印引入js方式

```jsx
document.write("<script type=\"text/javascript\" src=\"JustWalking.js\"></script>");
```















