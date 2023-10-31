>[!danger] 警告
> 实训课程所涉及的代码，如无特别说明，均要求手工输入，不可直接复制粘贴。

Tony 正准备骑着他地平衡车周游美国，我们准备帮他一把，为他在旅行者记录的日志改写成一张网页。

## 1.1 整理初始代码

这是未经加工的原始页面代码（可直接复制）：

```html
<html>
  <head>
    <title>My Trip Around the USA on a Segway</title>
  </head>
  <body>

    <h1>Segway'n USA</h1>
    <p>
      Documenting my trip around the US on my very own Segway!
    </p>

    <h2>August 20, 2012</h2>
    <img src="images/segway2.jpg">
    <p>
      Well I made it 1200 miles already, and I passed
      through some interesting places on the way:    
      Walla Walla, WA,Magic City, ID,Bountiful, UT,
      Last Chance, CO,Truth or Consequences and NM,Why, AZ.
    </p>
    
    <h2>July 14, 2012</h2>
    <p>
      I saw some Burma Shave style signs on the side of the
      road today:
    </p>
    <blockquote>
      Passing cars,
      When you can't see,
      May get you,
      A glimpse,
      Of eternity. 
    </blockquote>
    <p>
      I definitely won't be passing any cars.
    </p>

    <h2>June 2, 2012</h2>
    <img src="images/segway1.jpg">
    <p>
      My first day of the trip!  I can't believe I finally got
      everything packed and ready to go.  Because I'm on a Segway,
      I wasn't able to bring a whole lot with me:
      cellphone, iPod, digital camera, and a protein bar.
      Just the essentials.  As
      Lao Tzu would have said, <q>A journey of a 
      thousand miles begins with one Segway.</q>
    </p>
  </body>
</html>

```
这是网站上需要用到的图片：
![[151segway1.jpg]]
![[152segway2.jpg]]

>[!info] 任务 1：
> 请为 Tony 的网站建立一个文件夹，并用合理的形式组织网页相关文件的位置。提供的页面原始代码并不完全符合 HTML5 规范，请补充代码。

---
## 1.2 认识 `<q>` 和 `<blockquote>` 标签

>[!info] 任务 2：
> 在页面中找到运用了 `<q>` 和 `<blockquote>` 标签的代码，这两个标签都是表示“引用”，仔细观察后能否说出他们功能上的差别？

---
## 1.3 认识 `<br>` 标签

>[!info] 任务 3：
>  找到下面这段代码和页面上原始代码的区别，并在原网页中添加新增的标签。最后比较这两段代码执行后页面的不同之处，了解 `<br>` 标签的功能

```html
	<blockquote>
	  Passing cars, <br>
	  When you can't see, <br>
	  May get you, <br>
	  A glimpse, <br>
	  Of eternity. <br>
	</blockquote>
```

---
## 1.4 为页面添加列表

原始页面中有一段 Tony 8月份的的旅行记录，罗列了他踩着平衡车去过的城市：

```text
      Well I made it 1200 miles already, and I passed
      through some interesting places on the way:    
      Walla Walla, WA,Magic City, ID,Bountiful, UT,
      Last Chance, CO,Truth or Consequences and NM,Why, AZ.
```

但这种排版让人看起来非常吃力，能不能想办法改造这段文本，把各个城市排成一张列表，并在浏览器中以列表的形式显示出来呢？

这里我推荐 `<li>` 元素：
1. 第一步：将列表里的每一项都放在单独的 `<li>` 中。
2. 第二部：用 `<ol>` 或 `<ul>` 元素包围所有的 `<li>` 列表项。

>[!info] 任务 4：
>  找到页面中的城市列表部分，把每个城市都单列出来，改写成如下形式的有序列表。

```html
    <ol>
      <li>Walla Walla, WA</li> 
      <li>Magic City, ID</li> 
      <li>Bountiful, UT</li>
      <li>Last Chance, CO</li>
      <li>Truth or Consequences, NM</li>
      <li>Why, AZ</li> 
    </ol>
```

而 Tony 在 7 月份的旅行日志里，有一份行李清单

```text
      cellphone, iPod, digital camera, and a protein bar.
```

>[!info] 任务 5：
>  找到页面中的行李清单，改写成如下形式的无序列表。

```html
    <ul>
      <li>cellphone</li> 
      <li>iPod</li>
      <li>digital camera</li>
      <li>and a protein bar</li>
    </ul>
```