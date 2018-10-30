title: Markdown常用基本格式
date: 2018-10-29 10:21:01
tags: [Markdown]
mathjax: true  
<!-- 使用数学公式的开关 -->
categories: 杂七杂八


---

这是第一篇博客文章

主要分成以下几点来介绍
**1. Makedown语法**
**2. 使用感悟**

资源主要来源于以下文章：
> [Markdown常用格式](http://gaomf.cn/2015/10/30/Markdown%E5%B8%B8%E7%94%A8%E6%A0%BC%E5%BC%8F/#more)
> [markdown简明语法](http://ibruce.info/2013/11/26/markdown/)

本文所使用的Markdown解析器是Hexo附带的解析器进行讨论，其他Markdown解析器不在本文讨论范畴

<!--more-->

## 段落
段落有一个以上相连接的行句组成。  
若某一行只包含空格或者tab，则该行会被视为空行。
enter之后，转到下一个段落。

## 标题
使用1至6个`#`,对应1至6级标题
```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

```




## 分割线
使用3个以上`_`表示。
```markdown 
________
```
下面是用markdown得到的一条分割线
____
上面是用markdown得到的一条分割线

## 列表

### 无序列表
使用`-`,注意，`-`后有一个空格，不能省略，
```markdown
- 列表项1
- 列表项2
- 列表项3
```
- 列表项1
- 列表项2
- 列表项3

### 嵌套列表
交替使用`-` `+`, 并使用空格，进行缩进。
*注：Hexo支持两级嵌套。*
```markdown 
- 嵌套列表1
  + 嵌套列表11
  + 嵌套列表12
- 嵌套列表2
```

- 嵌套列表1
  + 嵌套列表11
  + 嵌套列表12
- 嵌套列表2

### 有序列表
使用`1.` `2.` `3.`,注意，使用之后，后面要跟一个空格
```markdown
1. 列表项1 
2. 列表项2 
3. 列表项3 

```
1. 列表项1 
2. 列表项2 
3. 列表项3 

## 引用
使用`>`表示
```markdown 
> 这是一条引用
```
> 这是一条引用

## 超链接
使用`[显示文本](链接地址)` ，该形式语法即可
```markdown
[浙江大学](http://www.zju.edu.cn)
[浙江理工大学](http://www.zstu.edu.cn/)
```

[浙江大学](http://www.zju.edu.cn)
[浙江理工大学](http://www.zstu.edu.cn/)
_____
也可以使用尖括号， 自动处理链接形式
```markdown
<http://17826855610@163.com>
<https://mail.163.com/js6/main.jsp?sid=zBgoiIQuYbFsSvKPaWuuwgiFGOvJKEJv&df=mail163_letter#module=mbox.ListModule%7C%7B%22fid%22%3A1%2C%22order%22%3A%22date%22%2C%22desc%22%3Atrue%7D>
```
<http://17826855610@163.com>
<https://mail.163.com/js6/main.jsp?sid=zBgoiIQuYbFsSvKPaWuuwgiFGOvJKEJv&df=mail163_letter#module=mbox.ListModule%7C%7B%22fid%22%3A1%2C%22order%22%3A%22date%22%2C%22desc%22%3Atrue%7D>

## 图片
使用`![](图片连接地址)`
```markdown 
![](http://t2.hddhhn.com/uploads/tu/201610/198/1oei3krh4ix.jpg)
```
![](http://t2.hddhhn.com/uploads/tu/201610/198/1oei3krh4ix.jpg)

## 文字粗体和斜体
前后使用2个`*`之后，中间包含一段文本，该文本为粗体文本；
前后使用1个`*`之后，中间包含一段文本，该文本为斜体文本
```markdown
这是正常文本
**这是粗体文本**
*这是斜体文本*
```
这是正常文本
**这是粗体文本**
*这是斜体文本*


## 表格
以下代码段，使用`:`来确定 对齐方式
```markdown
| Tables		| Are 			| Cool  |
|:----------:	|:-----:		|:-----:|
| col 3 is  	| centered  	| $1600 |
| col 2 is  	| right-aligned | $12	|
| zebra strips	| are neat		| $1	|
```
| Tables		| Are 			| Cool  |
|:----------:	|:-----:		|:-----:|
| col 3 is  	| centered  	| $1600 |
| col 2 is  	| right-aligned | $12	|
| zebra strips	| are neat		| $1	|

## 代码
### 行内代码
使用<code>\`</code> 包含代码片段。

### 代码段
使用<code>\`</code> 包含代码片段， 第一行的<code>\`\`\`</code>尾部可以指定使用的编程语言，建议手动设定，基本囊括所有常用语言	

|Language       | Alias |Language Name|Alias |
|:------------- |:----- |:------------|:-----|
|ARM assembler|armasm, arm|AVR assembler|avrasm|
|Awk|awk, mawk, nawk, gawk|Bash|bash, sh, zsh|
|Basic|basic|C#|cs, csharp|
|C, C++|cpp, c, cc, c++|CMake|cmake|
|CSS|css|DOS|dos, bat, cmd|
|Delphi, Pacal|delphi, pascal|Diff|diff|
|Django|django|DTS (Device Tree)|dts|
|Excel|excel|Fortran|fortran|
|Go|go|Gradle|gradle|
|Groovy|groovy|HTML, XML|xml, html, xhtml, rss|
|HTTP|http|JSON|json|
|Java|java|JavaScript|javascript, js|
|Lisp|lisp|Lua|lua|
|Makefile|makefile, mk, mak|Markdown|markdown, md|
|Matlab|matlab|PHP|php|
|Perl|perl|Processing|processing|
|Prolog|prolog|Python|python, py|
|R|r|Ruby|ruby|
|SQL|sql|Swift|swift|
|Tcl|tcl|TeX|tex|
|VB.Net|vbnet, vb|VBScript|vbscript, vbs|
|VHDL|vhdl|Verilog|verilog, v|
|Vim Script|vim|x86 Assembly|x86asm|

完整的帮助见：[CSS classes reference](http://highlightjs.readthedocs.io/en/latest/css-classes-reference.html)。如果不需要高亮，使用`no-highlight`

## 公式
需要[Mathjax](https://www.mathjax.org/)支持，详细说明来自[文档](http://mathjax.readthedocs.org/en/latest/)
Hexo本身不支持Mathjax插件，本博客系统使用的[Yilia](https://github.com/litten/hexo-theme-yilia)主题添加了Mathjax支持，故不需要做其它配置即可直接使用。Mathjax公式常用语法可参考:

> [Mathjax与LaTex公式简介](http://3iter.com/2015/10/14/Mathjax%E4%B8%8ELaTex%E5%85%AC%E5%BC%8F%E7%AE%80%E4%BB%8B/)

使用`$`表示行内公式， 使用`$$`表示整行公式，使用Latex格式编辑公式， 推荐一个好用的在线Latex公式可视化编辑器：[CodeCogs](https://www.codecogs.com/latex/eqneditor.php?lang=zh-cn)。下面为公式的实例效果。

_________

```markdown
质能方程：%E=mc^2$。其中$E$代表能量，$m$代表质量，$c$代表光速
```
质能方程：%E=mc^2$。其中$E$代表能量，$m$代表质量，$c$代表光速

```markdown
同样著名的麦克斯韦方程组为
$$\nabla\cdot\vec{B}=0$$
$$\nabla\cdot\vec{D}=\rho$$
$$\nabla\times\vec{H}=\vec{J} + \frac{\partial \vec{D}}{\partial t}$$
$$\nabla\times\vec{E}=- \frac{\partial \vec{B}}{\partial t}$$
此方程组由两个散度方程和两个旋度方程组成，是麦克斯韦方程组的微分形式，可转化为对应的积分形式：
$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=0$$
$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=\int\_{V}\rho \mathrm{d}V$$
$$\oint\_{l} \vec{H}\cdot \mathrm{d}\vec{l}=\int\_{S}(\vec{J}+\frac{\partial \vec{D}}{\partial t})\cdot\mathrm{d}\vec{S}$$
$$\oint\_{l} \vec{E}\cdot \mathrm{d}\vec{l}=-\int\_{S}\frac{\partial 
```
同样著名的麦克斯韦方程组为
$$\nabla\cdot\vec{B}=0$$
$$\nabla\cdot\vec{D}=\rho$$
$$\nabla\times\vec{H}=\vec{J} + \frac{\partial \vec{D}}{\partial t}$$
$$\nabla\times\vec{E}=- \frac{\partial \vec{B}}{\partial t}$$
此方程组由两个散度方程和两个旋度方程组成，是麦克斯韦方程组的微分形式，可转化为对应的积分形式：
$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=0$$
$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=\int\_{V}\rho \mathrm{d}V$$
$$\oint\_{l} \vec{H}\cdot \mathrm{d}\vec{l}=\int\_{S}(\vec{J}+\frac{\partial \vec{D}}{\partial t})\cdot\mathrm{d}\vec{S}$$


以上4个方程由两个散度方程和两个旋度方程组成，是麦克斯韦方程组的微分形式，可转化为对应的积分形式:

$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=0$$
$$\oint\_{S} \vec{B}\cdot\mathrm{d}\vec{S}=\int\_{V}\rho \mathrm{d}V$$
$$\oint\_{l} \vec{H}\cdot \mathrm{d}\vec{l}=\int\_{S}(\vec{J}+\frac{\partial \vec{D}}{\partial t})\cdot\mathrm{d}\vec{S}$$
$$\oint\_{l} \vec{E}\cdot \mathrm{d}\vec{l}=-\int\_{S}\frac{\partial \vec{B}}{\partial t}\cdot\mathrm{d}\vec{S}$$

_______
需要注意的是，正如[这篇文章](http://hijiangtao.github.io/2014/09/08/MathJaxinHexo/)所说，在书写MathJax公式的时候有时候会出现一些问题，主要是因为Markdown会将一些标记给编译掉，所以`_`、`{}`和`\\`等符号有时会出现问题，解决方式是在前面加上\进行转义。

## HTML标签
文本中可以直接使用html标签， 不需要额外标注这是 HTML 或是 Markdown，
只要区块元素——比如`<div>`、`<table>`、`<pre>`、`<p>`等标签， 必须前后加上空白，
以便于与内容相区分， 比如以下，可以居中放置一张图片， 其中url代表图片地址
```html
<div style="text-align: center">
<img src="url"/>
</div>
```
Html标签另外一个比较有用的作用是可以方便的直接插入一些符号，避免被Markdown解释器错误的解释。
