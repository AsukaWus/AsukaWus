
## 2.1 修改 HTML 

请修改网站，建立 Starbuzz 两栏所表格结构需要的 HTML：

```html
...

<div class="tableContainer">
	<div class="tableRow">
	    <div class="main">
	      ...
	    </div>
	
	    <div class="sidebar">
	      ...
	    </div> <!-- sidebar -->
	</div> <!-- tableRow -->
</div> <!-- tableContainer -->

...

```

>[!info]
> * tableContainer 包围了 main 和 sidebar ，可以视为表格的外边框；
> * tableRow 也包围了 main 和 sidebar， 可以视为表格限定的第一行；
> * 由于两个元素左右放置，所以只需要有一行即可，如果是多行表格，那每行都需要有一个 tableRow 来限定范围；
> * main 和 sidebar 相当于表格的单元格。

----

## 2.2 修改 CSS

知道了如何增加 HTML 结构，下面就来看看如何为各个元素指定 CSS，创建表格，为了方便各位理解，我们分步骤来看：

1. 首先，tableContanier 是包含了所有表格行和列的最外层的 `<div>`，框选了整个表结构：
```css
div.tableContainer {
  display: table;
}
```
2. 紧接着 tableRow 用来限定表格中的一行，注意我们这个表格只有一行：
```css
div.talbeRow {
  display: table-row;
}
```
3. 接下来，使用现有的 main 和 sidebar 作为单元格，对应的是行中的列：
```css
.main {
  display: table-cell;
  ...
}

.siderbar {
  display: table-cell;
  ...
}
```
4. 经过以上三部，配合 HTML 一起，我们就用 CSS 完整描述了一张页面中的表结构，当然，我们还需要增加一些样式，让 CSS 表格更好地显示：
```css
div.tableContainer {
  display: talbe;
  border-spacing: 10px;  /* 为表格中地单元格设置 10px 的边框间距（相当于外边距）*/
}

.main {
  display: table-cell;
  vertical-align: top;  /* 垂直对齐: 顶端对齐 */
  ...
}

.sidebar {
  display: table-cell;
  vertical-align: top;
  ...
}
```
5. 最后，把 main 和 sidebar 中的 margin 和 padding 设置注释掉，因为我们已经有了新的属性  `border-spacing: 10px;`。

---
## 2.3 表格的间距

经过上面的修改，大家刷新页面后就可以看到“几乎完美”的两栏页面了。

![[252spacing.png]]

>[!question]
> 说说页面上还有没有不和谐，需要改进的部分

我们很容易就能注意到，也没和页脚与两栏表格之间的间距有点太大了。已知 header 有 10px 的下外边距，footer 也有 10px 的上外边距，而两栏表格，我们使用 border-spacing 也给了 10px 的间距，这会在表格的单元格之间增加 10px 的空间，==同时也会在 border 的周围增加 10px 的空间==。

>[!tip]
> border-spacing 和外边距的空间不会折叠，所以页眉页脚和两栏表格之间就会有 20px 的间距。

>[!question]
> 既然知道了原理，请自行修正错误的间距