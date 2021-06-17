# blogIt

找个后端小项目做做，弄个小博客，前端偷个懒，从别人的成果开始，前端fork自[Aimee](https://github.com/Aimee1608/myblogvue),感谢！

如果有前端有新的想法大家也可以一起改造一波。我这边打算弄java做个后端。

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

项目变更说明
- 开发时的跨域问题
>假如是在同一台机器上开发，前后端分离的工程中出现跨域问题的原因是，前端工程和后端工程运行在不同的端口上。只要协议、域名、端口有一个不同就会产生跨域问题，所以在前端工程中请求后端的接口时就会因为端口不同而产生跨域问题。

前端不能直接访问跨域的地址，比如前端运行在8080端口，那么发出的请求地址也必须是8080,不能是8081,否则跨域，那么如果想要访问8081的后端接口咋办。
使用代理，将8080上该路径的接口代理到8081端口上去，
