Starbuzz 的 CEO 对你的页面非常满意，决定再为页面增加一列，，提供饮料单，他希望新的这一列放在 main 的左侧，宽度是浏览器窗口的 20%，新增内容中与表格布局无关的代码如下：

```html
<div class="drinks">
	<h1>BEVERAGES</h1>
	<p>House Blend, $1.49</p>
	<p>Mocha Cafe Latte, $2.35</p>
	<p>Cappuccino, $1.89</p>
	<p>Chai Tea, $1.85</p>
	<h1>ELIXIRS</h1>
	<p>
		We proudly serve elixirs brewed by our friends
		at the Head First Lounge.
	</p>
	<p>Green Tea Cooler, $2.99</p>
	<p>Raspberry Ice Concentration, $2.99</p>
	<p>Blueberry Bliss Elixir, $2.99</p>
	<p>Cranberry Antioxidant Blast, $2.99</p>
	<p>Chai Chiller, $2.99</p>
	<p>Black Brain Brew, $2.99</p>
</div>
```

这部分和布局无关的 CSS 如下：

```css
.drinks {
    background-color: #efe5d0;
    padding: 15px;
}
```

>[!question]
>请你根据已经写好的 HTML 完成 CSS 样式的设置，实现三栏效果。

![[253three.png]]