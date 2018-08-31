---
title: Hexo之二配置
p: hexo/config.md
date: 2018-08-31 21:21:36
tags:
 - hexo
categories:
 - 工具
 - 博客
 - hexo
---

在`_config.yml`中设置配置

<!-- more -->

## 网站

| 参数 | 描述 |
| --- | --- |
| title | 网站标题 |
| subtitle | 网站副标题 |
| description | 网站描述 |
| author | 作者 |
| language | 网站语言 |
| timezone | 网站时区，如America/New_York, utc，默认为电脑时区 |

## 网址

| 参数 | 描述 |
| --- | --- |
| url | 网址 |
| root | 网站根目录 |
| permalink | 文章的永久链接格式，默认为:year/:month/:day/:title/ |
| permalink_defaults | 永久链接中各部分的默认值 |

如果网站存放在子目录中，例如 http://yoursite.com/blog，则将 url 设为 http://yoursite.com/blog 并把 root 设为 /blog/

permalink中可使用的变量

| 变量 | 描述 |
|---|---|
| :year | 年份YYYY |
| :month | 月份MM |
| :i_month | 月份M |
| :day | 日期DD |
| :i_day | 日期D |
| :title | source中的文章路径, 如hexo/README |
| :post_title | 文章标题 |
| :id | 文章ID |
| :category | 分类 |

## 目录

| 参数 | 描述 |
| --- | --- |
| source_dir | 资源文件夹，用于存放资源，默认为source |
| public_dir | 公共文件夹，用于存放生成的站点文件，默认为public |
| tag_dir | 标签文件夹，默认为tags |
| achieve_dir | 归档文件夹，默认为archieves |
| category_dir | 分类文件夹，默认为categories |
| code_dir | include code 文件夹，默认为downloads/code |
| i18n_dir | 国际化文件夹，默认为:lang |
| skip_render | 跳过渲染指定文件，可使用glob表达式来匹配路径 |

## 文章

| 参数 | 描述 |
| --- | --- |
| new_post_name | 新文章的文件名称，默认为:title.md |
| default_layout | 默认布局，默认为post |
| auto_spacing | 中文和英文之间自动加入空格，默认为false |
| titlecase | 把标题转换为title case，默认为false |
| external_link | 在新标签中打开链接，默认为true |
| filename_case | 文章名称转换为小写(1)或大写(2)，默认为0 |
| render_drafts | 渲染草稿，默认为false |
| post_asset_folder | 启动Assert文件夹，默认为false |
| relative_link | 将链接改为基于根目录的相对地址，默认为false |
| future | 显示未来的文章，默认为true |
| highlight | 代码块设置 |

## 分类&标签

| 参数 | 描述 |
| --- | --- |
| default_category | 默认分类，默认为uncategorized |
| category_map | 分类别名 |
| tag_map | 标签别名 |

## 日期/时间格式

| 参数 | 描述 |
| --- | --- |
| data-format | 日期格式，默认为YYYY-MM-DD |
| time-format | 时间格式，默认为HH:mm:ss |

## 分页

| 参数 | 描述 |
| --- | --- |
| per_page | 每页显示的文章数，默认为10 |
| pagination_dir | 分页目录，默认为page |

## 扩展

| 参数 | 描述 |
| --- | --- |
| theme | 当前主题，值为false禁用主题 |
| deploy | 部署 |

## 默认配置

```yml
# Hexo Configuration
## Docs: https://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/

# Site
title: 网站标题
subtitle: 网站副标题
description: 网站描述
author: 作者
language: zh-cn
timezone:

# URL
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: http://www.wchaochao.com
root: /
permalink: :year/:month/:day/:title/
permalink_defaults:

# Directory
source_dir: source
public_dir: public
tag_dir: tags
archive_dir: archives
category_dir: categories
code_dir: downloads/code
i18n_dir: :lang
skip_render:

# Writing
new_post_name: :title.md # File name of new posts
default_layout: post
titlecase: false # Transform title into titlecase
external_link: true # Open external links in new tab
filename_case: 0
render_drafts: false
post_asset_folder: false
relative_link: false
future: true
highlight:
  enable: true
  line_number: true
  auto_detect: false
  tab_replace: 2
  
# Home page setting
# path: Root path for your blogs index page. (default = '')
# per_page: Posts displayed per page. (0 = disable pagination)
# order_by: Posts order. (Order by date descending by default)
index_generator:
  path: ''
  per_page: 10
  order_by: -date
  
# Category & Tag
default_category: uncategorized
category_map:
tag_map:

# Date / Time format
## Hexo uses Moment.js to parse and display date
## You can customize the date format as defined in
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss

# Pagination
## Set per_page to 0 to disable pagination
per_page: 10
pagination_dir: page

# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: landscape

# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type:

```