---
title: GitHub上使用Hexo建立博客
date: 2016-03-07 13:59:29
tags:
---

  目标：使用Hexo生成静态文件，上传GitHub作为博客。
  
## 搭建环境

### 下载安装node.js
  到[Node.js](https://nodejs.org)官网[下载](https://nodejs.org/en/download/)相应平台的最新版本，一路安装即可。

### 下载安装Git，创建GitHub账号，上传SSH-KEY。
  具体内容参考[此博客](http://ibruce.info/2013/11/22/hexo-your-blog/)。
  注意: GitHub新建仓库名：github账号.github.io
        博客访问地址： http://github账号.github.io

### 安装Hexo
``` bash
$ git config --global core.autocrlf false
$ npm install --unsafe-perm --verbose -g hexo //安装在 \Users\用户名\AppData\Roaming\npm\node_modules目录下
```
## 初始化

### 生成博客文件
```bash
$ hexo init MyBlog
$ cd MyBlog
$ hexo generate //生成静态页面
```

### 本地启动
  执行如下命令，启动本地服务，预览文章。
```bash
$ hexo server
```
  在浏览器输入[http://localhost:4000](http://localhost:4000)就可以看到效果。