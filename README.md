## rs
### 如水博客hugo主题
博客地址:https://rushui.net
## 使用方式
```bash
hugo new site blog -f yaml 
cd blog
git init
git submodule add https://github.com/hugo-theme/rs.git themes/rs
echo "theme: rs" >> config.yaml
hugo server
```
## 保留目录
blog中所有目录都是空的，所以只保留用到的目录和文件即可
```bash
content #内容目录
static #静态文件目录
themes #主题目录
config.yaml #配置文件
```
## 添加内容
```bash
hugo new posts/blog-quickstart.md
```
posts/blog-quickstart.md 加入以下内容
```bash
---
title: "用hugo快速创建一个博客"
date: 2023-03-04T17:53:26+08:00
tags : ["如水"]
---
这是通过如水博客主题模板创建的内容。
```
### 启动服务
```bash
hugo server -D
```
打开 http://localhost:1313/ 即可看到刚才加的内容