---
title: hexo-renderer-kramed行内渲染错误解决方法
date: 2019-09-10 22:51:09
categories:
- [Linux, Hexo]
tags:
- Hexo
---

摘要：修改转义符号的转义规则，解决语义冲突，使行内LaTeX公式正常渲染。

<!--more-->

测试版本：

```bash
hexo: 3.9.0
hexo-renderer-kramed: 0.1.4
kramed: 0.5.6
```

在hexo根目录下，找到 `\node_modules\kramed\lib\rules\inline.js` ，第11行改为：

```javascript
escape: /^\\([`*\[\]()#$+\-.!_>])/
```

第20行修改为：

```javascript
em: /^\*((?:\*\*|[\s\S])+?)\*(?!\*)/
```

重新生成博客。
