---
layout: post
title: 看iOS开发玩 Node.js - 零,一切的开始
excerpt: A brief use of Node.js. 帮助你开始Node.js之旅
categories: tools
---

@author 周宇 [Email](jou@oenius.com) [Weibo](http://weibo.com/monfur) or [Github](https://github.com/oenius)

***

# 看iOS开发玩 Node.js - 零,一切的开始

## 预热 - Full Stack Developer

> 移动互联网时代，依我感觉是一个快速学习的时代。如何快速掌握一项技能，并应用于实践，绝对是一个值得探讨的话题。
> 而我相信多数的计算机科学家（就像美术，不愿意被称为美工一样，我也该称自己是计算机科学家），也都怀揣着一颗全栈的心。
> 爱Full Stack 就不能少了 Full Stack Language. - JavaScript.
> Node.js 是js的服务器端应用。 在 游戏服务器，RESTFul api的方面 都有很好的表现， 当然Node.js的应用场景不限于这些。
> 我的理解，学语言就像开始一段恋爱，有的无法自拔，有的情深缘浅。而我与Node.js更有种相见恨晚的感觉。


## ECMAScript 2015 (ES6) in Node.js

WTF， 不是说好Javascript吗？！

更多教程 [ECMAScript 6简介](http://es6.ruanyifeng.com/#docs/intro)

## 安装NVM (Node version manager)
像Ruby 的RVM (Ruby version manager) 一样, 给Node安装一个版本管理器.

安装nvm需要打开命令行窗口，运行下面的命令。（示例代码是v0.31.0）

```
  curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash
```

然后 active nvm

```  
  source ~/.nvm/nvm.sh

```

更多文档 [GitHub](https://github.com/creationix/nvm/blob/master/README.markdown)

## 安装Node

```
nvm install node

```

安装指定版本

```

nvm install 5.0

```

查看安装版本

```

nvm ls

```

使用指定版本

```

nvm use 5.0

```



## Let's say "Hello world"

抛去差异性较大的环境配置。假设已经安装好了Node.js。

创建文件server.js

``` server.js
  var http = require('http');

   http.createServer(function (request, response){
       response.writeHead(200,{'Content-Type':'text/plain'});
       response.end('Hello World');
   }).listen(8081);

   console.log('Server running at 127.0.0.1:8081');

```

因为Node.js帮助我们实现了整个HTTP服务器。所以为了run 这个server并不需要类如Apache 或者 Nginx 的HTTP 服务器。

打开终端，运行代码

```  

node server.js
Server running at http://127.0.0.1:8081/

```

## REPL(交互式解释器)

在终端的交互解释器， 在帮助入门上有很大的帮助。使用上，和python, ruby,swift没有特别的地方。

ctrl + c两次 退出REPL


***
