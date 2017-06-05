## 为什么学习并使用Vue
>
>1.发展趋势
>
>
最近这几年的前端圈子，由于戏台一般精彩纷呈，从 MVC 到 MVVM，你刚唱罢我登场。 backbone，AngularJS 已成昨日黄花，reactjs 如日中天，同时另一更轻量的 vue 发展势头更猛，号称兼具了 angularjs 和 reactjs 的两者优点。
>
>
>2.Vue能干吗
>
>
移动端的上网需求已经远高于pc端，特别是 hybrid 方式的H5应用中，但是性能问题一直是痛点。 如果使用 SPA（就是俗称的单页应用（Single Page Web Application）），SPA它将所有的活动局限于一个Web页面中，仅在该Web页面初始化时加载相应的HTML、JavaScript 和 CSS。一旦页面加载完成了，SPA不会因为用户的操作而进行页面的重新加载或跳转。没有页面切换，就没有白屏阻塞，可以大大提高 H5 的性能，达到接近原生的流畅体验。
>
>
陆续续看vue已经二个多月了，3月份使用vue2.0开发了一个简单的博客，在用vue人性化优势的同时，的也遇到过很多坑，很多问题，分享一下我遇到的问题和解决办法
陆

## Vue2_blog
>
> vue2,vuex,vue-cli,axios,webpack,express,mysql 
## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080 (本地启动)
npm run dev

# build for production with minification （生成静态文件，用于打包上传服务器）
npm run build
```
## 主要实现的功能
>
1.用户登录
>
2.用户注册
>
3.用户发帖
>
4.用户评论帖
>
5.用户留言

## 构建
>
>使用vue-cli来构建初始化项目，非常方便，相当于生成项目模板这样子。

## vuex 
>
>vue就我个人理解，是数据驱动，实现页面组件化开发，更好管理和维护，vuex是用作组件间的通信，当然了如果页面够简单，也可以使用其他方法进行通信（传值），比如props等。

## axios
>
>说实话，项目前期我还用的是vue-resource，后面才统一改用axios（尤大大本人都力推的），二者都是用于客户端和服务端通信的，也就是用作ajax请求的。

## webpack
>
>webpack是一款模块加载器兼打包工具，它能把各种资源，例如JS（含JSX）、coffee、样式（含less/sass）、图片等都作为模块来使用和处理。比如，我们vue组件化开发，会用 ".vue" 文件，这种文件不会被浏览器所解析，所以需要用webpack来 "格式化" 他们，让他们变为浏览器可以解析的文件格式。还有，还有，用webpack，你就可以愉快的使用es6的语法啦！

## express & mysql
>
>所谓一个"系统"，怎么只能是简单的静态页面？在这里用了express（express 是一个基于 Node.js 平台的开发框架）和mysql来进行编写数据存储的后端api，用于用户信息在数据库里存储和读取。
## pm2
>
>pm2 是一个带有负载均衡功能的Node应用的进程管理器,并保证进程永远都活着，0秒的重载。按照我的理解，通俗的将，它的作用就是，本地开发环境，你要开启node服务，实现某些功能(比如监听某个端口)，就会在控制台执行"node app.js"(比如这个文件叫app吧！)，对应的node服务就会开启了，但是你只要一关闭这个控制台窗口，他就没有对应的服务进程了，每次起服务都得"控制台 -> node app.js"。在生产环境来说，很麻烦，这会就用到了pm2，只需要执行一次"pm2 start app.js"。ok，一劳永逸，控制台窗口随你怎么自由开启关闭，对应的服务进程永远在后面运行着。
>
## 项目预览
>
[Vue_blog](https://www.zygg.cc)
>
## 总结
>
>刚用vue开发的时候，遇到了很多问题，也犯了很多错误，不过，现在而言，自己收获蛮多。自己的vue博客（留言板）已经开发完成。我想说的是，麻雀虽小，五脏俱全，虽然只是一个小应用，但它涵盖了许多知识点，包括前端，后端，数据库等一个网站的所必须的一些组成要素，对我来说，学习意义很大，愿共勉！
