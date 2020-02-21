---
layout: post
title: "如何自定义jekyll-theme"
date: 2020-2-20
category: explore
---

[jekyll教程][jekyll-tutorial]


出于想要自己写模板以及样式来个性化自己的博客的目的，亟需了解目录结构以及各目录的作用。

当我们安装jekyll的时候就默认自带了主题minimal，该主题文件夹在

`\Ruby25-x64\lib\ruby\gems\2.5.0\gems\minima-2.5.1`


之前还在纠结为什么网上下载的主题的目录结构和我`new jekyll myblog`之后生成的目录格式大不相同，原来那些缺少的主题文件都放在这。
```
 ├── LICENSE.txt
 ├── README.md
 ├── _includes--存放模板页面需要用到的部分 | 方便通过{{- include.footer -}}来引用
 │   ├── disqus_comments.html
 │   ├── footer.html
 │   ├── google-analytics.html
 │   ├── head.html
 │   ├── header.html
 │   ├── icon-github.html
 │   ├── icon-github.svg
 │   ├── icon-twitter.html
 │   └── icon-twitter.svg
 ├── _layouts--存放模板页面的文件夹 | 在post的FrontMatter部分即最前面`---`使用`layout:default就`能够指定母版页
 │   ├── default.html
 │   ├── home.html
 │   ├── page.html
 │   └── post.html
 ├── _sass--存放css样式表
 │   ├── minima
 │   │   ├── _base.scss
 │   │   ├── _layout.scss
 │   │   └── _syntax-highlighting.scss
 │   └── minima.scss
 └── assets
     └── main.scss
```


[jekyll-tutorial]:https://jekyllrb.com/docs/step-by-step/02-liquid/