---
layout: post
title: 看iOS开发玩 Node.js 之入门篇
excerpt: A brief use of Node.js. 帮助你开始Node.js之旅
categories: tools
---

#看iOS开发玩Node.js 之入门篇

## 预热 - Full Stack Developer

> 互联网时代，绝对是一个快速学习的时代。如何快速掌握一项技能，并应用于实践，绝对是一个值得探讨的话题。
> 我的理解，学语言就像开始一段恋爱，有的无法自拔，有的情深缘浅。
> 而我相信多数的计算机科学家（我更愿意称我们是计算机科学家），怀揣着一颗全栈的心。
> 爱Full Stack 更爱 Full Stack Language. - JavaScript.

## Let's say "Hello world"

抛去差异性较大的环境配置。假设已经安装好了Node.js。

```
  var http = require('http');

   http.createServer(function (request, response){
       response.writeHead(200,{'Content-Type':'text/plain'});
       response.end('Hello World');
   }).listen(8888);

   console.log('Server running at 127.0.0.1:8888');

```
