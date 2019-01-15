# Vue-router
通过监听`window.location.hash`（也就是`domain:port/a/b#/A/B`）中的`#/A/B`变化来切换视图。

## work flow
- 规划好路由结构
  - 有哪些path？
  - 有哪些路由参数？
  - 嵌套路由的时候，父子路由的关系
- 每个路由上面有哪些组件？
  - 组件的树状图？
  - 组件之间需要交流吗？
  - 完成组件
    - 静态组件
    - 传值组件
    - ajax组件

## code flow
- 创建路由对象
- 明确路径和组件的对应关系
- 在根实例注册路由
- 编写对应组件

## SPA
- main
  - router1
    - component1
    - component2
    - component3
  - router2
    - componentA
    - routerA
    - routerB
      - componentB
  - router3

## [router-link](./router-link.md)

## [路由跳转时组件的生存情况](./life.md)

## 动态参数
``` js
{
  path: '/user/:id',
  component: user
}
```
在路由中这样定义，然后当页面处于符合上述正则规则的路由的时候，可以通过`this.$route.params.id`来调用

## 多重嵌套
同时，本次实例中，`/pl/:language/projects/:num`中，language的变化不会销毁再创建子路由`projects/:num`。但是会触发子路由中的一些钩子函数 比如你可以watch $route。num的变化也会触发pl.vue中相应的构造函数。

## [note](./detail.md)

## [conclusion](./conclu.md)

## Build Setup

``` bash
npm install
npm run serve
```
