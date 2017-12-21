---
title: 初探json-server
comments: true
date: 2017-12-14 11:42:16
tags: mockdata
categories: mockdata
---
## 起因

   前端有三痛：1、与产品经理打交道，每天改改改；2、与后端打交道，由于产品改导致后端数据改改改；3、与QA打交道，每天问你为什么不这样做，大哥，去问产品噻。产品和QA的问题目前没有好的解决方案，对于后端数据由于产品修改不能及时给出mockdata的问题，顺藤摸瓜找到了json-server。

## 实例

  node、npm必备的工具，在这里就不赘述了。

  开发环境与工具：windows下git bash。

   1、全局安装json-sever
     `npm install -g json-server` 
     遇到的问题： 在git bash下安装报错，需要在管理员权限下安装。
   2、创建db.json文件，输入以下内容
    `{
	  "student": [
	    {"id": 1, "name": "zhangsan", "age":"18", "gender": "male"},
	    {"id": 2, "name": "lisi", "age": "20", "gender": "female"}
	  ]
	}`  

   3、输入命令 
	   `json-server db.json`  
	    可以看到如下：
	   {% asset_img result.jpg  %}  
   4、打开浏览器输入：http://localhost:3000/student，可以看到如下效果：
	   {% asset_img render.jpg %}


