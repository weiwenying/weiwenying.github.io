---
layout: post
title:  "10_使用Github Pages搭建博客"
date:   2016-03-15
excerpt: "可以使用jekyll搭建一个个人小站，需要网页前端编程基础。"
tag:
- 03_Git的相关
comments: false
---


# Kramdown的语法

Kramdown 是markdown的一种扩展版本，github支持这种语法显示。

## 基本元素

### 标题

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

最多为六级标题。

### 图片的显示

```markdown
../images2013-06-25-10_使用Github Pages搭建博客/01_测试的图片.png
```

显示结果如下：

![01_测试的图片.png](../images/2013-06-25-10_使用Github Pages搭建博客/01_测试的图片.png)

### 网络链接

```markdown
[www.google.com](www.google.com)
```

显示结果如下：

[www.google.com](www.google.com) 

### 引用说明

```markdown
> 鲁迅说：要呐喊！
```

显示效果如下：

>   鲁迅说：要呐喊！

### 序列号

```markdown
- 思想自由
- 言论自由
- 新闻自由
```

显示如下：

- 思想自由
- 言论自由
- 新闻自由

序号号：

```markdown
1.  人民当家做主。
2.  人民是主人。
3.  人民公仆，公务员是仆人。
```

显示结果如下：

1.  人民当家做主，人民是主人。
2.  人民公仆，公务员是仆人。
3.  主人被仆人禁言，这是不科学的。

### 表格

```markdown
| 法治     | 民主     | 和谐     | 富强     |
| -------- | -------- | -------- | -------- |
| 有吗？   | 有吗？   | 有吗？   | 有吗？   |
| 你确定？ | 你确定？ | 你确定？ | 你确定？ |
```

显示结果如下：

| 法治     | 民主     | 和谐     | 富强     |
| -------- | -------- | -------- | -------- |
| 有吗？   | 有吗？   | 有吗？   | 有吗？   |
| 你确定？ | 你确定？ | 你确定？ | 你确定？ |

## 视频显示

下面，我们将添加一个视频链接的显示，代码如下：

```markdown
<iframe width="560" height="315" src="//www.youtube.com/embed/SU3kYxJmWuQ" frameborder="0"> </iframe>
```

这其实是使用了HTML标签，将 `www.youtube.com/embed/SU3kYxJmWuQ` 这个视频（如果你没有科学上网，可能无法看到下面加载的youtube视频），显示如下：

<iframe width="560" height="315" src="//www.youtube.com/embed/SU3kYxJmWuQ" frameborder="0"> </iframe>

这样，视频就可以在当前页面下播放了。同时，可以设置视频占据页面的大小， [FitVids](http://fitvidsjs.com/) 这个网址会教你如何设置。

## 数学公式

数学公式使用的是 [MathJax](http://www.mathjax.org/) 插件，支持 Tex/LaTex/MathML 这些HTML简化版语言。比如，下面写法：

```latex
$$
a = \sum_{i = 0}^{a}{x_i}
$$
```
显示结果如下:

$$
a = \sum_{i = 0}^{a}{x_i}
$$


MathJax官方没有特别详细的说明，可以使用 [katex官方教程](https://katex.org/docs/supported.html) ，语法差不多。