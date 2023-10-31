现在我们有了一个包围了饮料区所有元素的 `<div>`，好戏开场，我们可以对他指定样式。请在对应的 lounge.css 文件中增加规则。

>[!danger] 警告
> 课程所涉及的代码，如无特别说明，均要求手工输入，不可直接复制粘贴。

## 2.1 增加边框

仅仅增加 div 在页面上是体现不出变化的，我们先给这个饮料分区增加边框，把 div 凸显出来

```css
.elixirs {
	border-width: thin;
	border-style: solid;
	border-color: #007e7e;
}
```

完成后，页面上的饮料分区就应该有了边框。

___
## 2.2 处理宽度

让 elixirs 分区变窄，设计成一个书签式的细长宣传单的样子。

```css
.elixirs {
	...
	width: 200px; /* width 属性允许指定内容区的宽度 */
}
```

>[!danger] 警告
> 注意了看注释，是内容区 content 的宽度，想想看为什么要特别强调这一点。

>[!tip] 
> 去浏览器调整下窗口的宽度，看看这个“书签”宽度受不受影响。

关于 width 的更多说明：

1. 一个  block 元素的默认宽度是 auto，也就是占满整行的空间。
2. 如果没有 padding, margin, border 那元素的宽度就是 width 的宽度。

>[!tip] 
> 一般来讲，元素的高度应该是默认的 auto，浏览器会在垂直方向上延伸内容区，使区块中的所有元素可见，当你设置 width 为 200px 后，饮料区明显长高了，这就是 auto 在起作用。
>
> 当然，你也可以试着区指定一个高度 height，但这样做风险很大，一旦高度不够，放不下所有的元素，那么多余的元素会“溢出”到其他区块或元素中，引起页面混乱。

>[!question]
> 显然，elixirs 因为还有 padding，margin，border 的存在，不可能宽度为 200px，那它真正的宽度是多少？

---
## 2.3 增加边距

边距是老朋友了，不解释：

```css
.elixirs {
	...
	padding-right:   20px；
	padding-bottom:  20px;
	padding-left:    20px;
	
	margin-left:     20px;
}
```

___
## 2.4 设置背景并文本居中

```css
.elixirs {
	...
	background-image:    url(images/cocktail.gif);
	background-repeat:   repeat-x;

	text-align:          center;  /* 文本剧中对齐 */
}
```

text-algin 是和我们首次见面，主要用于文本对齐，对齐方式有左对齐，居中对齐和右对齐。此时请打开网页观察我们设置的上述 CSS 是否起效。

>[!tip] 
> 你应该发现却可能没有发现：text-align 又是一个可以被子元素继承的样式。当然，并不是所有的样式属性都能被继承，请不要忘记以前学过的旧知识。
