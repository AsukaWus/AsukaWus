我们都已经知道了 class 是分类，对应的是多个页面元素，那么示例代码中作为页面唯一元素的却归类的做法就显得有点突兀了：

```html
    <p class="guarantee">
      Our guarantee: at the lounge, we're committed to providing you, 
      our guest, with an exceptional experience every time you visit. 
      Whether you're just stopping by to check in on email over an 
      elixir, or are here for an out-of-the-ordinary dinner, you'll 
      find our knowledgeable service staff pay attention to every detail. 
      If you're not fully satisfied, have a Blueberry Bliss Elixir on us.
    </p>
```

>[!info] 任务9
> 请把 HTML 中的 class 改成 id 观察页面变化。

显然因为选择器的问题，页面中的对应段落目前丢失了我们用两节课设置好的样式。

>[!info] 任务 10
> 修改 CSS 中的对应的选择器，让样式重新生效。