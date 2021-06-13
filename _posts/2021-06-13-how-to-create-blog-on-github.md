---
layout: post
title: 如何在GitHub上创建个人博客
---

<p class="message", style="background-color: #e64980;">
  👋 嗨！这篇文章是介绍如何在GitHub上创建个人博客
</p>

在GitHub上面创建博客的过程其实和发布repo是一样的。

## Github

- 先访问自己Github主页（如果没有需要注册哦~）
- 找到新建Repositories，也就是界面左侧有一个绿色的New符号，点击创建
- 进入后选择输入Repository name，需要注意的是必须严格按照 *username.github.io* 格式，username为你的用户名
- 选择Create repository即可完成创建
- 此时访问 `https://username.github.io` 即可（但是没有对应的内容，即为空白）

## Jekyll

- jekyll是一个生成静态网页的工具，可以免费部署在我们刚刚创建的repo上
- 但是想要熟练的使用jekyll还是需要一些学习时间。如果想要快速创建博客的话，可以先fork别人的代码，再自行调整和学习。
- 这是公开的jekyll主题网站:[jekyll-themes](http://jekyllthemes.org/)，可以去上面选择自己喜欢的主题进行fork
- 我本人选择的是[dark-poole](http://jekyllthemes.org/themes/dark-poole/)
- 将代码下载到本地即可

## Build

- 为了先体验一下，代码中的作者信息等等可以稍后再修改
- 因为涉及到commit等操作，我个人建议下载[Github-Desktop](https://desktop.github.com/)来方便进行资源管理
- 登录Desktop后，将我们刚刚创建的repo复制下来（可自定义clone文件），绑定git方便后续管理
- 将下载的代码复制进入本地的repo文件
- 此时Desktop上的左侧Changes会显示发生的改变 
- 选择左下侧的 `commit to master` 提交更改，再选择界面上方的push即可完成推送

## View
- 此时，再访问`https://username.github.io`时，界面已经变成我们所选择的主题
- 后续，再按照类似的方法对本地文件进行修改commit后再push即可
- 在jekyll中，一般配置文件为 `_config.yml`，因此通常修改改文件可以满足大多数自定义要求
- 如果想要提交自己的文章，通常则是由`_posts`文件夹进行管理
- 更多具体内容可以查看fork代码中的Readme以及jekyll官方教程[jelyll](https://jekyllrb.com/)