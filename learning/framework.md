## 1. props 在[Vue](https://cn.vuejs.org/)、[React](https://zh-hans.reactjs.org/)中的区别？

> - `vue`中的`props`支持传递静态或动态`props`，静态`props`一般传递字符串。
> - `react`中的`props`是一个从外部传进组件的参数，主要作为就是从父组件向子组件传递数据，它具有可读性和不变性，只能通过外部组件主动传入新的`props`来重新渲染子组件，否则子组件的`props`以及展现形式不会改变。