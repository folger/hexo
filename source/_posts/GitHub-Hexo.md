---
title: GitHub + Hexo
date: 2016-04-26 15:56:46
tags:
---

### 一篇好文章

[使用GitHub和Hexo搭建免费静态Blog](http://wsgzao.github.io/post/hexo-guide/)

### 重点步骤

- 安装 [node.js](http://nodejs.org)
- 运行以下命令准备好hexo
    ```bash
    npm install -g cnpm --registry=https://registry.npm.taobao.org
    npm install hexo-cli -g
    npm install hexo --save
    npm install hexo-deployer-git --save
    ```
- hexo init或者git clone已有的 [hexo repo](https://github.com/folger/hexo)
- 主要的hexo命令
    ```bash
    hexo new
    hexo server
    hexo generate
    hexo deploy
    ```
