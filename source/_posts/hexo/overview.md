---
title: Hexo之一概述
p: hexo/overview.md
date: 2018-08-29 21:49:12
tags:
 - hexo
categories:
 - 工具
 - 博客
 - hexo
---

* 基于`NodeJS`环境的博客框架
* 使用`Markdown`或其他渲染引擎解析文章
* 利用主题生成静态网页

<!-- more -->

## 安装

* 安装`Nodejs`：基于NodeJS环境
* 安装`Hexo`：npm安装

```bash
$ npm install -g hexo-cli
```

## 初始化

```bash
// 初始化Hexo博客
$ hexo init <folder>

// 安装依赖
$ cd <folder>
$ npm install
```

初始化完成后，文件夹目录如下

```
├── .deploy         # 需要部署的文件
├── node_modules    # Hexo插件
├── public          # 生成的静态网页文件
├── scaffolds       # 模板
├── source          # 博客正文和其他源文件，404、favicon、CNAME 都应该放在这里
| ├── _drafts       # 草稿
| └── _posts        # 文章
├── themes          # 主题
├── _config.yml     # 全局配置文件
└── package.json    # npm 依赖等
```