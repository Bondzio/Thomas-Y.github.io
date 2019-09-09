---
title: Hexo中插入图片的通用方法
date: 2019-09-08 21:50:50
categories:
- [Tools, Hexo]
tags:
- Hexo
---

摘要：通过修改permalink设置，可以只使用Markdown通用语法，使图片在atom编辑器、hexo首页、hexo文章页均正常显示。

<!--more-->

默认情况下，`source` 和 `public` 文件夹的文件结构（忽略部分文件）为

```
public
├── year
│   └── month
│       └── day
│           └── title
│               └── index.html
├── images
│   └── image.png
└── index.html

source
├── images
│   └── image.png
└── _posts
    └── title.md
```

对于少量图片，官方文档建议的方法放在 `source/images` 中，按照类似 `![](/images/image.png)` 的形式访问。

考虑到以上方法无法在Atom中编辑时显示图片，尝试使用相对路径 `![](../images/image.png)` 。此时，查看首页图片的链接为 `http://yoursite.com/images/image.png` 可以正常显示，文章内图片的链接为 `http://yoursite.com/year/month/day/images/image.png` 无法正常显示。

显然，只要修改文章 `permalink` 设置使相对路径可以指向图片正确位置即可。在  `_config.yml` 中找到

```
permalink: :year/:month/:day/:title/
```
修改为
```
permalink: :year:month:day-:title/
```

重新生成博客，此时 `public` 文件夹的文件结构（忽略部分文件）变更为

```
public
├── :year:month:day-:title
│   └── index.html
├── images
│   └── image.png
└── index.html
```

查看首页图片和文章内图片链接均为 `http://yoursite.com/images/image.png` 可以正常显示。
