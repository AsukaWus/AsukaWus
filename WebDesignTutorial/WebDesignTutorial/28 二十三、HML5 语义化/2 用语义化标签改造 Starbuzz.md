如果你之前严格按照我的文档完成页面的话，现在的网页结构应该是如下这样的：
```html
<div id="header">
</div>

<div id="award">
</div>

<div id="tableContainer">
	<div id="tableRow">
		<div id="drinks">
		</div>
		<div id="main">
		</div>
		<div id="sidebar">
		</div> <!-- sidebar -->
	</div> <!-- tableRow -->
</div> <!-- tableContainer -->

<div id="coupon">
</div>

<div id="footer">
</div>
```

## 2.1 HTML5 改造
在学习了语义化的 html5 标记之后，请对他们进行改造：

```html
 <header class="top">
 </header>

<div id="tableContainer">
	<div id="tableRow">
		<section id="drinks">
		</section>
		<section id="main">
		</section>
		<aside>
		</aside>
	</div> <!-- tableRow -->
</div> <!-- tableContainer -->

<footer>
</footer>
```

>[!warning]
> 如果不出意外的话，页面应该是要出意外了，试讨论原因。

___
## 2.2 为元素更新 CSS