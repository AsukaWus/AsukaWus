页面的流式布局 Flow 是 HTML 的默认布局形式，所以也是最常用的布局形式，相信通过前文的例子各位已经能够理解 Flow 和 float 为页面带来的改变了。

lounge 休闲吧网站已经陪伴了各位一段时间，所以从今天开始要换换口味，接下来的课程为大家准备了一个全新的 Starbuzz 咖啡店宣传网站：

![[starbuzz.zip]]

大家不妨下载后看看这个网站的初始架构。

## 2.1 观察页面

在浏览器中打开页面，找到以下四个部分：

1. 页眉：包含 Starbuzz 的公司 logo 以及公司宗旨的说明；
2. 文字介绍区：包含了一些关于 Starbuzz 的介绍，历史严格，产品介绍的文字区域；
3. 单品广告区：正在用图片和文字结合的形式推销一种名为 Bean Machine 的新咖啡豆，甚至还有一个指向了购买页面的链接；
4. 页脚：毫无新意的 Copyright 声明。

---
## 2.2 查看 HTML

页面的 HTML 部分非常友好，对页面中的四个部分都用 `<div>` 单独区分，规划划好了页面的逻辑。我把这个基本结构复制了过来：

```html
	<div id="header">

	</div>

	<div id="main">
     
	</div>

	<div id="sidebar">
 
	</div>

    <div id="footer">

    </div>
```

我们可以看到 4 个分区都已经起好了自己的名字：

1. 页眉：     header;
2. 文字介绍区：main;
3. 单品广告区：sidebar;
4. 页脚：     footer.


>[!question]
> 这是网站的原始代码，用 id 并不妥当，请自行修改成 class。

___
## 2.3 确认样式

>[!tip]
> 在 vscode 中打开样式表应该能获得更好的阅读体验，请在开始动手前确认，有没有自己不了解的css 属性或属性值，请和小组同学讨论，消灭盲点。

```css
body { 
  background-color: #b5a789;
  font-family:      Georgia, "Times New Roman", Times, serif;
  font-size:        small;
  margin:           0px;
}

#header {
  background-color: #675c47;
  margin:           10px;
  height:           108px;
}

#main {
  background:       #efe5d0 url(images/background.gif) top left;
  font-size:        105%;
  padding:          15px;
  margin:           0px 10px 10px 10px;
}

#sidebar {
  background:       #efe5d0 url(images/background.gif) bottom right;
  font-size:        105%;
  padding:          15px;
  margin:           0px 10px 10px 10px;
}

#footer {
  background-color: #675c47;
  color:            #efe5d0;
  text-align:       center;
  padding:          15px;
  margin:           10px;
  font-size:        90%;
}

h1 {
  font-size:        120%;
  color:            #954b4b;
}

.slogan { color: #954b4b; }

.beanheading {
  text-align:       center;
  line-height:      1.8em;
}

a:link {
  color:            #b76666;
  text-decoration:  none;
  border-bottom:    thin dotted #b76666;
}
a:visited {
  color:            #675c47;
  text-decoration:  none;
  border-bottom:    thin dotted #675c47;
}
```