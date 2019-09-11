---
title: Markdown语法学习笔记
date: 2019-09-09 16:04:50
categories:
- [Tools, Markdown]
tags:
- Markdown
---

摘要：Markdown标准语法；示例；使用技巧。

<!--more-->

<!-- TOC START min:1 max:3 link:true asterisk:false update:true -->
- [1 标题](#1-标题)
- [2 段落](#2-段落)
- [3 字体样式](#3-字体样式)
- [4 分隔线](#4-分隔线)
- [5 列表](#5-列表)
- [6 代码](#6-代码)
	- [代码片段](#代码片段)
	- [代码块](#代码块)
- [7 链接](#7-链接)
- [8 图片](#8-图片)
- [9 表格](#9-表格)
<!-- TOC END -->

# 1 标题

用 `#` 号标记，一级标题对应一个 `#` 号，二级标题对应两个 `#` 号，以此类推。

```markdown
# 一级标题
## 二级标题
### 三级标题
```

# 2 段落

在段落后面使用一个空行或两个空格加回车来表示重新开始一个段落。

```markdown
第一段

第二段
```

或

![效果](../images/20190909-markdown-learning-note/2-effect.png)


# 3 字体样式

```markdown
*斜体文本*

**粗体文本**

***粗斜体文本***

~~带删除线文本~~

<u>带下划线文本</u>
```

显示效果：  
*斜体文本*

**粗体文本**

***粗斜体文本***

~~带删除线文本~~

<u>带下划线文本</u>

# 4 分隔线

```markdown
---
```

# 5 列表

```markdown
* 第一项
* 第二项
* 第三项

1. 第一项
2. 第二项
3. 第三项

* 第一项
	1. 第一项嵌套的第一个元素
	2. 第一项嵌套的第二个元素
```

显示效果：

* 第一项
* 第二项
* 第三项

1. 第一项
2. 第二项
3. 第三项

* 第一项
	1. 第一项嵌套的第一个元素
	2. 第一项嵌套的第二个元素

# 6 代码

## 代码片段

```markdown
`printf()` 函数
```

显示效果：  
`printf()` 函数

## 代码块

````markdown
```javascript
$(document).ready(function () {
    alert('RUNOOB');
});
```
````

显示效果：  
```javascript
$(document).ready(function () {
    alert('RUNOOB');
});
```

# 7 链接

```markdown
链接[github](https://github.com)
```

显示效果：  
链接[github](https://github.com)

# 8 图片

```markdown
![效果](../images/20190909-markdown-learning-note/8-effect.png)
```

显示效果：  
![效果](../images/20190909-markdown-learning-note/8-effect.png)

# 9 表格

```markdown
| 左对齐 | 右对齐 | 居中对齐 |
|:------ | ------:|:--------:|
| 1      |      2 |    3     |
```

显示效果：

| 左对齐 | 右对齐 | 居中对齐 |
|:------ | ------:|:--------:|
| 1      |      2 |    3     |

注：为防止渲染问题,表格前后最好空一行。
