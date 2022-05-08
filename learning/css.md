## 1. visibility=hidden, opacity=0，display:none 区别？

> opacity=0，该元素隐藏起来了，但不会改变页面布局，并且，如果该元素已经绑定一些 事件，如 click 事件，那么点击该区域，也能触发点击事件的 visibility=hidden，该元素 隐藏起来了，但不会改变页面布局，但是不会触发该元素已经绑定的事件 display=none， 把元素隐藏起来，并且会改变页面布局，可以理解成在页面中把该元素删除掉一样。

## 2. CSS 中 link 和@import 的区别是什么？

> - `link`属于 HTML 标签，而`@import`是 CSS 提供的
> - 页面被加载的时，`link`会同时被加载，而`@import`被引用的 CSS 会等到引用它的 CSS 文件被加
>   载完再加载
> - `import`只在 IE5 以上才能识别，而`link`是 HTML 标签，无兼容问题
> - `link`方式的样式的权重 高于`@import`的权重
