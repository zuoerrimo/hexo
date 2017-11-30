---
title: 不可不知的javascript身世
comments: true
date: 2017-11-28 15:30:14
tags: js
categories: javascript重撸之旅
---

## javasrcipt与java的关系

  在当时，java很火，javasrcipt想蹭java的热度，所以才得名javascript。

## javasrcipt与ECMAScript的关系

  ECMAScript是javascript的标准，javacript是ECMAScript的实现。
  

## 解释型语言与编译型语言

   - 解释型语言：单句翻译，速度稍微慢些，跨平台 代表： javascript、php
   - 编译型语言：通篇翻译，速度稍微快些，不跨平台，代表： C、C++
   - java是借助jvm是在跨平台的，所以不属于上述两种
   - javasrcipt是单线程的(划重点)
     js是单线程的，浏览器是多线程的。[参考链接](http://www.cnblogs.com/Mainz/p/3552717.html)

## javascript的组成

   DOM + BOM + ECMAScript

## 主流浏览器及其内核

  | 浏览器        | 内核           | 
| ------------- |:-------------:| 
| IE      | trident |
| Chrome    | webkit/blink（V8替换掉JSCore）      | 
| Safari     | webkit/blink      |   
| firefox | Gecko      | 
| Opera | presto      | 


