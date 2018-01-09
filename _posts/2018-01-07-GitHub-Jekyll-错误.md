---
layout: post
title: "在GitHub使用Jekyll构建个人博客时出现的错误"
author: "wanlihon"
header-img: "img/post-bg-cuowu.jpg"
categories: posts rwd
permalink: /:categories/:title.html
tags:
    - GitHub
    - Jekyll
    - 网页设计与制作
---

在GitHub使用Jekyll构建个人博客时出现的错误
====
**CNAME错误**  
[关于CNAME已经采取问题详解](https://help.github.com/articles/troubleshooting-custom-domains/#cname-already-taken)  
- 出现这个错误的原因

```
您在GitHub Pages网站的存储库设置中添加或编辑自定义域时，我们会自动在您的存储库的根目录中创建一个CNAME文件。CNAME文件中的自定义域只能使用一次
```
- 解决这个错误的方法
1. 打开你的文件夹中
2. 找到CNAME文件
3. 删除它  
  
**symlink错误**  
[关于页面构建失败：文件是一个符号链接的错误详解](https://help.github.com/articles/page-build-failed-file-is-a-symlink/)
-出现这个错误的原因  

```
如果你的GitHub Pages版本库中的文件引用了一个不存在于你的版本库中的符号链接文件，那么你的GitHub Pages网站将不会生成
```
- 解决这个错误的方法
1. 找到出现这个错误的文件并打开
2. 查找(快捷键Ctrl+F)include
3. 检查关于include代码是否有链接到不存在的文件（你的文件名打错啦）。
4. 更改或删除就可以啦

```
以上仅为我目前遇到的错误和解决办法，不适用于全部人，如有错误或不足，欢迎指正。
```

