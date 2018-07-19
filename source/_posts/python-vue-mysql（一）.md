---
title: python+vue+mysql（一）
comments: true
date: 2018-07-17 15:37:33
tags: python、vue
categories: python、vue
---

## 起因
  
   每天用着同事的组件、后端的数据，七拼八凑的写着绵延不绝的业务代码，觉得工作索然无味，应该被安排一下。

## 开整
    
    开发环境与工具： win10、git bash、Sublime Text，node、npm这些当然是必备了就不一一列举咯。

    ### mysql安装
    
        google mysql安装，映入眼帘的是mysql教程-菜鸟教程，按照文档中window环境下的安装步骤进行

          * 为了避免每次用mysql时，都要切换到mysql/bin目录下，需要配置mysql的环境变量

    ### python 

        参考廖大神的pythoy的教程，当然我的目标是能够通过python实现数据库的CRUD操作。
        大致的看了一下基本语法，直接进入到访问数据库mysql篇章。

        * 踩坑：python连接数据库代码就绪后，运行报如下错误：
          {% asset_img mysql.pngs %}
          解决办法：[答案]( https://blog.csdn.net/mimica247706624/article/details/5986546 "答案")

    ### vue

        vue-cli初始化项目，创建一个python目录，编写app.py文件用于查询数据库。

    ### 合体，一起打天（阿修罗梗）

        合体过程中遇到了跨域问题，身为前端的我肯定是想从前端解决，找了配置文件中proxyTable属性进行配置，可是行不通。想了想从后端解决吧，搜到了flask_cors，问题解决了。

    [项目参考链接](https://github.com/zuoerrimo/python-vue"项目参考链接")