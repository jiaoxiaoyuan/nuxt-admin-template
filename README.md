# nuxt-element-admin

> 基于 Nuxt.js 服务渲染框架搭建的后台管理系统，UI 框架选择的是[Element UI](https://element.eleme.cn/#/zh-CN)

> 该后台管理系统只是一个极简的后台基础模板，只实现了用户登录和权限验证等功能。

## 参考文档

- [基于 Nuxt.js 服务渲染框架的后台管理系统](https://github.com/JanesChan/Vue-admin)
- [vue-element-admin](https://panjiachen.github.io/vue-element-admin-site/zh/guide/)

## 前期准备

> 项目搭建参考另一篇文章：[nuxt-koa-mongodb](https://github.com/zptime/nuxt-koa-mongodb)

项目创建差异：

- 创建框架时，UI 框架选择[Element UI](https://element.eleme.cn/#/zh-CN)
- 未进行 pwa 的额外配置
- 未进行 mongodb 数据库的相关配置
- 增加sass/scss 配置

```js
// 安装
npm i node-sass sass-loader scss-loader --save-dev
npm install @nuxtjs/style-resources

// 配置 nuxt.config.js
styleResources: {
  // 全局混入scss
  scss: '~assets/css/mixins.scss'
}
```

## 页面编写

- pages/login/index.vue 页面：登录页面
- layouts/base.vue：基础框架页，不带任何组件的框架页
- layouts/default.vue：主要框架页，带侧边栏和顶栏的框架页

```js
// store/index.js
npm install js-cookie
```
