## 2.1 五种 font-family 字体系列

### 2.1.1 衬线体
衬线体字体带有一些小的“线条”或“尾巴”，如宋体、Times New Roman等。这些线条有助于人眼识别和跟踪字形，使得长篇文字阅读更易于阅读和理解。

>[!tip]
> 衬线体适合用于印刷品和长篇阅读，如书籍、报纸等。

<div style="font-family: Times; font-size:2em">Times</div>
<div style="font-family: 'Times New Roman'; font-size:2em">Times New Roman</div>
<div style="font-family: Georgia; font-size:2em">Georgia</div>
<div style="font-family: '宋体'; font-size:2em">宋体</div>
<div style="font-family: '新宋体'; font-size:2em">新宋体</div>

---
### 2.1.2 非衬线体
非衬线体字体没有这些线条或尾巴，如 Arial、等线 等。非衬线体字体在小字号下更易于阅读，因为没有额外的细节来干扰阅读。

>[!tip]
> 非衬线体更加简单、现代，适合用于数字媒体、网页设计等方面。

<div style="font-family: Verdana; font-size:2em">Verdana</div>
<div style="font-family: 'Arial Black'; font-size:2em">Arial Black</div>
<div style="font-family: Arial; font-size:2em">Arial</div>
<div style="font-family: '微软雅黑'; font-size:2em">微软雅黑</div>
<div style="font-family: '等线'; font-size:2em">等线</div>

---
### 2.1.3 等宽字体
等宽字体指每个字符占据相同的宽度，适用于排版等宽排列的代码、表格等内容，可提高可读性。等宽字体与程序代码和计算机技术等相关领域有着密切的关系。

>[!tip]
> 是程序员和开发人员的首选字体之一。我这篇文档就是 Cascadia Mono 做默认字体。

<span style="font-family: 'Cascadia Mono'; font-size:2em">Cascadia Mono </span>  <span style="font-family: 'Cascadia Mono'; font-size:2em">/ 1lL0Oo,:;.</span>
<span style="font-family: 'Cascadia Code'; font-size:2em">Cascadia Code </span> <span style="font-family: 'Cascadia Code'; font-size:2em"> / 1lL0Oo,:;.</span>
<span style="font-family: 'Courier New'; font-size:2em">Courier New </span> <span style="font-family: 'Courier New'; font-size:2em"> / 1lL0Oo,:;.</span>
<span style="font-family: 'Consolas'; font-size:2em">Consolas </span> <span style="font-family: 'Consolas'; font-size:2em"> / 1lL0Oo,:;.</span>

>[!warning]
> 1. 等宽字体未必每个字都绝对等宽。
> 2. 相比英文字体而言，中文字体大部分都等宽。


---
### 2.1.4. 手写体
手写体字体是一种仿制手写字体的字体，它们的笔画、连线和变化等仿制手写字体的特点，形成了一种自然、亲切、人性化的效果。

>[!tip]
手写体字体往往适用于需要营造个人化、手工、艺术感的设计，如个人书信、明信片、海报等。

<div style="font-family: 'Segoe Script'; font-size:2em">Segoe Script</div>
<div style="font-family: 'Segoe Print'; font-size:2em">Segoe Print</div>
<div style="font-family: 'Comic Sans MS'; font-size:2em">Comic Sans MS</div>
<div style="font-family: '华文行楷'; font-size:2em">华文行楷</div>
<div style="font-family: '华文新魏'; font-size:2em">华文新魏</div>

---
### 2.1.5 装饰字体
装饰字体是一种带有艺术气息的字体，具有非常鲜明的特色，用于设计时可以起到烘托气氛的作用。这类字体常常采用华丽的线条、弯曲的线条和非常夸张的效果。

>[!tip]
> 装饰字体可用于设计宣传品、海报、广告和一些与艺术相关的设计。

<div style="font-family: 'French Script MT'; font-size:2em">French Script MT</div>
<div style="font-family: 'Book Antiqua'; font-size:2em">Book Antiqua</div>
<div style="font-family: '华文琥珀'; font-size:2em">华文琥珀</div>
<div style="font-family: '华文彩云'; font-size:2em">华文彩云</div>

___
## 2.2 指定 font-family

```css
body {
	font-family: Verdana, Geneva, 'Arial';
}
```

font-family 往往不会止指定一个字体，而是包含一个来自于同一个字体系列的字体列表。

>[!question]- Question 1：为什么是列表？
> 答：
> 	1. 这是为了防止对方用户计算机上没有相应的字体，本例中就会首先尝试用 Verdana 展示，如果 Verdana 不可用，则尝试 Geneva 字体，依次类推。
> 	2. 最后一个 Arial 是保底策略，一般都会选择非常常见的系统自带字体，保证显示效果。
> 	3. 出现在首位的 Verdana 字体应该是设计者最想让用户看到的字体呈现。
> 	4. 建议为字体名称加上引号，因为有很多字体是由多个单词组成的词组，比如 "French Script MT"

>[!question]- Question 2：为什么要同一个字体系列？
>答：使用同一字体系列的不同字体作为备选字体是为了保证整个页面的视觉统一性，以确保在某种字体无法正常显示的情况下，使用备选字体来替代的同时保持整体风格一致。

---
## 3.3 使用网络字体（略）

[Google Fonts | 谷歌字体中文版 | GoogleFonts](https://www.googlefonts.cn/fonts)

