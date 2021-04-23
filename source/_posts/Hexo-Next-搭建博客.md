---
title: Hexo+Next 搭建博客
tags:
  - Blogs
categories:
  - Blogs
date: 2021-04-22 16:04:44
---

#### 前言
博主首次创建个人Blogs，首篇文章主要分享下博客搭建过程
博客环境主要用**Hexo+Next**搭建，用**gitee**码云部署
<!-- more -->

#### Hexo安装与配置

- 具体配置可以看[Hexo中文官网文档](https://hexo.io/zh-cn/)
- 开始前请确认自己已安装Node和Git相关工具

安装Hexo脚手架
```
$ npm install -g hexo-cli
```

直接安装hexo项目
```
$ cd <folder>
$ npm install
```

然后主要配置在根目录下的_config.yml里面配置即可

#### NexT主题优化

在项目根目录下，执行以下命令
```
$ git clone https://github.com/theme-next/hexo-theme-next themes/next
```

在项目根目录下打开_config.yml文件将theme设置为next
主题的配置可以在 /theme/next/_config.yml 里面配置

> 主题具体配置可以上Next的文档查阅或者参考这篇文章[NexT优化博客](https://blog.csdn.net/wugenqiang/article/details/88373990)

然后执行命令即可运行
```
$ hexo serve
// 或者
$ hexo s
```

#### Gitee安装部署

参考文档[Hexo + Gitee安装部署完整过程](https://blog.csdn.net/daniel_wangt/article/details/107201959)

> 注意：在最后打包项目包上传的时候如果出现 “ERROR Deployer not found: git” 的报错<br>安装以下依赖即可
```
$ npm install --save hexo-deployer-git
```
