---
title: hexo 部署
date: 2016-04-07 22:58:05
tags:
---
想搭建一个个人博客，又没有主机服务器的屌丝来说，[github pages](https://pages.github.com/)是一个不错的选择。github推荐使用[Jekyll](https://jekyllrb.com/)，用ruby开发的一个框架，由于本人最近在使用nodejs，所以选择了[hexo](https://hexo.io/)，下文记录了hexo的安装过程。

### 安装nodejs
[nodejs](https://nodejs.org/en/)是一个基于Chrome JavaScript运行时建立的平台， 用于方便地搭建响应速度快、易于扩展的网络应用。从官网下载安装包，安装过程不再详细叙述。

### 安装hexo

``` bash
$ npm install-g hexo
```
{% img /img/20160407/1.png 1394 956  %}

### 部署hexo

新建一个文件夹blog，初始化应用。
``` bash
$ mkdir blog
$ cd blog
$ hexo init
```
{% img /img/20160407/2.png 1394 956  %}