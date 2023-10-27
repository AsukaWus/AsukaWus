在之前的课程中，我们已经尝试过利用 font-weight 属性来修改字体的粗细。

```css
body {
	font-weight: bold;
	font-weight: 400;
}
```

## 4.1 关键字形式
我们可以使用 font-weight 属性预设的关键字来设置字体的粗细，例如:

	1. bold
	2. normal
	3. lighter
	4. bolder

其中，bold 表示粗体，normal 表示正常字体（即普通字体），lighter 表示比 normal 更细的字体，bolder 表示比 bold 更粗的字体。

## 4.2 数值形式

也可以使用 font-weight 属性的数值来设置字体的粗细，数值范围是 100 到 900，数值越大，字体越粗，==其中 400 等价于关键字 normal，700 等价于关键字 bold==。

## 4.3 其他形式

除了以上两种常用形式之外，在字体文件中，通常会包含多个不同粗细的字体，可以通过在 CSS 中引用相应的字体文件来实现不同粗细的字体。就拿微软雅黑来说，根据粗细就有多个字体版本，包括：

*   Microsoft YaHei: 常规的微软雅黑字体，也是默认字体。
*   Microsoft YaHei Bold: 粗体版本。
*   Microsoft YaHei Light: 细体版本，线条较为纤细。
*   Microsoft YaHei UI: 更新版本，字重相对于常规版更轻，字体设计更加平滑。
*   Microsoft YaHei UI Bold: Microsoft YaHei UI 的粗体版本。
*   Microsoft YaHei UI Light: Microsoft YaHei UI 的细体版本。
