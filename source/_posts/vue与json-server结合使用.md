---
title: vue与json-server结合使用
comments: true
date: 2017-12-21 10:55:03
tags: mockdata
categories: mockdata
---
 
 ## 起因

   之前学习vue时，一直在想怎么更好的展现数据，而不需要用java、php等后端语言，有很多办法用expres与mongodb做结合是我最近一直想做的，但为了简单选择了json-server做基础数据开发。

## 实例

   1、安装vue-cli、json-server

   2、`vue init webpack vue-json-server-demo`

   3、在vue-json-server-demo创建文件夹mock,mock下创建mock.js,如图：
       {% asset_img mockjs.jpg %}

   4、在package.json中添加`"mock": "json-server mock/mock.js --port 9090",`命令

   5、由于mock.js中有用到faker、lodash，我们需要输入`npm install faker lodash --save`

   6、`npm run mock`,浏览器中输入http://localhost:9090/people，可以看到一组json字符串

   7、最终想实现如下的效果
     {% asset_img userlist.jpg %}

   8、将src/components/HelloWorld.vue作为我们要展示的页面

   9、安装axios用于请求数据，`npm install axios --save`

   10、安装element-ui用于页面展示,`element-ui`

   11、main.js中添加element-ui的引用，如下图
       {% asset_img mainjs.jpg %}

   12、配置mock的代理，在config/index.js中配置代理如图：
       {% asset_img proxy.jpg %}
       这样访问api/xxx就可以直接跳转到9090上访问。当然也可以同时配置axios的baseUrl设置代理，
       如图：
       {% asset_img base.pngs %}

   13、HelloWorld.vue逻辑代码如下： 
       {% asset_img hello.jpg %}

    