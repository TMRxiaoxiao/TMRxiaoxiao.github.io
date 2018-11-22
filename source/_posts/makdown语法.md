---
title: markdown语法
date: 2018-11-22 10:06:57
tags: 技术
---

---

| 功能     | 快捷键   |
| -------- | -------- |
| 加粗     | Ctrl + B |
| 斜体     | Ctrl + I |
| 引用     | Ctrl + Q |
| 插入链接 | Ctrl + L |
| 插入代码 | Ctrl + K |
| 插入图片 | Ctrl + G |
| 提升标题 | Ctrl + H |
| 有序列表 | Ctrl + O |
| 无序列表 | Ctrl + U |
| 横线     | Ctrl + R |
| 撤销     | Ctrl + Z |
| 重做     | Ctrl + Y |

> 推荐使用typora

---
<!--more-->


# 1.标题<a name="top"></a>

> 标准语法一般在#后跟个空格再写文字。

```markdown
# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题
```

# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题

# 2.分级标题

> `=` `-` 最少可以只写一个，兼容性一般

```markdown
一级标题
======================
二级标题
---------------------
```

一级标题
======================
二级标题
---------------------

# 3.TOC

> 根据标题生成目录，兼容性不好

```markdown
[TOC]
```

[TOC]

# 4.引用

+ 单行

````markdown
> hello world
````

> hello world 

+ 多行

````markdown
> hello world
hello world
hello world

或者
> hello world 
> hello world 
````

> hello world
> hello world
> hello world



> hello world 
> hello world 

+ 多层嵌套

````markdown
> aaaaaaaaa
>> bbbbbbbbb
>>> cccccccccc
````

> aaaaaaaaa
> > bbbbbbbbb
> >
> > > cccccccccc

# 5.行内标记

> 用 ` 标记**代码块将变成一行**

```markdown
标记之外`hello world`标记之外
```

标记之外`hello world`标记之外

# 6.代码块

> 与上行距离一空行

~~~markdown
```
<div>   
    <div></div>
    <div></div>
    <div></div>
</div>
```
~~~

```html
<div>   
    <div></div>
    <div></div>
    <div></div>
</div>
```

# 7.插入链接

> `{:target="_blank"}`跳转方式兼容性一般 ，多数第三方平台不支持跳转

```markdown
[百度1](http://www.baidu.com/" 百度一下"){:target="_blank"} 
```

[百度1](http://www.baidu.com/" 百度一下"){:target="_blank"} 

```markdown
[百度2][2]{:target="_blank"}
[2]: http://www.baidu.com/   "百度二下"
```

[百度2][2]{:target="_blank"}

[2]: http://www.baidu.com/   "百度二下"

# 8.任务列表

> 兼容性一般 要隔开一行

```markdown
这是文字……

- [x] 选项一
- [ ] 选项二  
- [ ]  [选项3]
```

- [x] 选项一
- [ ] 选项二  
- [ ] [选项3]

# 9.表格

>  代表对齐方式 ,** `:` 与 `|` 之间不要有空格**，否则对齐会有些不兼容

````markdown
|    a    |       b       |      c     |
|:-------:|:------------- | ----------:|
|   居中  |     左对齐    |   右对齐   |
|=========|===============|============|
````

|     a     | b               |            c |
| :-------: | :-------------- | -----------: |
|   居中    | 左对齐          |       右对齐 |
| ========= | =============== | ============ |



````markdown
a  | b | c  
:-:|:- |-:
    居中    |     左对齐      |   右对齐    
============|=================|=============
````

|      a       | b                 |             c |
| :----------: | :---------------- | ------------: |
|     居中     | 左对齐            |        右对齐 |
| ============ | ================= | ============= |

# 10.嵌套css样式

```markdown
<p style="color: #AD5D0F;font-size: 30px; font-family: '宋体';">内联样式</p>
```

<p style="color: #AD5D0F;font-size: 30px; font-family: '宋体';">内联样式</p>



# 11.语义标记

| 描述      | 效果          | 代码              |
| --------- | ------------- | ----------------- |
| 斜体      | *斜体*        | `*斜体*`          |
| 斜体      | *斜体*        | `_斜体_`          |
| 加粗      | **加粗**      | `**加粗**`        |
| 加粗+斜体 | **加粗+斜体** | `***加粗+斜体***` |
| 加粗+斜体 | **加粗+斜体** | `**_加粗+斜体_**` |
| 删除线    | ~~删除线~~    | `~~删除线~~`      |

# 12.语义标签

| 描述     | 效果                                                         | 代码              |
| -------- | ------------------------------------------------------------ | ----------------- |
| 斜体     | <i>斜体</i>                                                  | `<i>斜体</i>`     |
| 加粗     | <b>加粗</b>                                                  | `<b>加粗</b>`     |
| 强调     | <em>强调</em>                                                | `<em>强调</em>`   |
| 上标     | Za                                                           | `Z<sup>a</sup>`   |
| 下标     | Za                                                           | `Z<sub>a</sub>`   |
| 键盘文本 | ![img](https:////upload-images.jianshu.io/upload_images/6912209-9f4177c5bfb69ab0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/47/format/webp) | `<kbd>Ctrl</kbd>` |
| 换行     |                                                              | ``                |

# 13.公式

> 1个$左对齐，2个居中

```markdown
$$ x \href{why-equal.html}{=} y^2 + 1 $$
$ x = {-b \pm \sqrt{b^2-4ac} \over 2a}. $
```

$$ x \href{why-equal.html}{=} y^2 + 1 $$
$ x = {-b \pm \sqrt{b^2-4ac} \over 2a}. $

# 14.分隔符

> 最少三个 `---` 或 `***`或 `* * *`

```markdown
***
---
* * *
```

***
---
* * *



# 15.脚注

```markdown
Markdown[^1]
[^1]: Markdown是一种纯文本标记语言        // 在文章最后面显示脚注
```

Markdown[^1]

# 16.锚点

> 只有**标题**支持锚点， 跳转目录方括号后 保持空格

```markdown
[公式标题锚点](#1)

### [需要跳转的目录] {#1}    // 方括号后保持空格
```

[顶部](#top)



>
>
>> 1. 添加链接: 通过添加标签 < a>标题一< /a>
>
>​	2.添加锚点: 在需要跳转到的标题位置添加链接
>​	< a name="锚点名称">标题一< /a>
>
>​	3.修改1中的标签< a href="#要跳转到的锚点名称">标题一< /a>

# 17.自动邮箱链接

```markdown
<tmrsmile@outlook.com>
```

<tmrsmile@outlook.com>

# 18.流程图

````markdown
​```flow                     // 流程
st=>start: 开始|past:> http://www.baidu.com // 开始
e=>end: 结束              // 结束
c1=>condition: 条件1:>http://www.baidu.com[_parent]   // 判断条件
c2=>condition: 条件2      // 判断条件
c3=>condition: 条件3      // 判断条件
io=>inputoutput: 输出     // 输出
//----------------以上为定义参数-------------------------

//----------------以下为连接参数-------------------------
// 开始->判断条件1为no->判断条件2为no->判断条件3为no->输出->结束
st->c1(yes,right)->c2(yes,right)->c3(yes,right)->io->e
c1(no)->e                   // 条件1不满足->结束
c2(no)->e                   // 条件2不满足->结束
c3(no)->e                   // 条件3不满足->结束
​```
````

```flow
st=>start: 开始
e=>end: 结束             
c1=>condition: 条件1
c2=>condition: 条件2      
c3=>condition: 条件3      
io=>inputoutput: 输出     
st->c1(yes,right)->c2(yes,right)->c3(yes,right)->io->e
c1(no)->e                   
c2(no)->e                 
c3(no)->e         
```









