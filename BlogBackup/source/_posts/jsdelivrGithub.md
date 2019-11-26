---
title: 使用jsDelivr在GitHub上打造CDN库

author: Mashiro

avatar: https://cdn.jsdelivr.net/gh/MashiroRb/CDNjsDelivr@v1.6/img/custom/Avatar.png

authorLink: https://mashiro.fun/

authorAbout: 呐 你想变成什么颜色？

authorDesc: 呐 你想变成什么颜色？

categories: 极客

date: 2019-11-25 11:37:41

comments: true

tags: 

 - CDN

keywords: jsDelivr

description: jsDelivr+GitHub

photos: https://cdn.jsdelivr.net/gh/MashiroRb/CDNjsDelivr@v1.8/img/banner/tqzz.jpg

---



## jsDelivr

> Jsdelivr 网站是一个致力于为开发者提供数千种Javascript、CSS等超过1650多种 Libraries加速的免费CDN服务，该平台是首个「打通中国大陆与海外的免费CDN服务」，网页开发者无须担心中国防火墙问题而影响使用。 
jsDelivr平台将服务重心放在更快速的网路连线，利用CDN技术来确保每个地区的使用者都能获得最好的连接速度。此外jsDelivr可将不同的JavaScript或CSSlibraries整合在一起，通过一段链结来载入网站，非常方便!
> 如果你正在寻找类似服务，jsDelivr 是个不错的选择。

## 配置过程

### 1、新建GitHub库

### 2、安装git
#### git官方下载：[这里这里](https://git-scm.com/)
#### macOS建议使用homebrew安装：
```git
# 安装homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 安装git
brew install git
```

### 3、使用git上传本地文件到GitHub
1.本地新建一个文件夹
2.使用终端定义到该目录(windows系统鼠标右键git bash here)
3.终端输入`git init`
4.复制GitHub仓库git地址
例如`https://github.com/MashiroRb/CDNjsDelivr.git`
5.输入
```git
git remote add origin 刚才复制的地址

git pull origin master
```
6.将要上传的文件放入该文件夹
7.输入
```git
git add .

# 添加内容描述
git commit -m '添加内容描述'

# 将本地文件上传到GitHub
git push origin master
```
### 4、建立releases联系
进入GitHub仓库，找到`release`,然后点击`Draft a new release`,建立release之后记住版本号。
找到该仓库里要使用的资源，例如`https://github.com/MashiroRb/CDNjsDelivr/blob/master/img/logo/Google.svg`
假如你的版本号是v1.8，此时使用jsDelivr调用的结果就是`https://cdn.jsdelivr.net/gh/MashiroRb/CDNjsDelivr@v1.8/img/logo/Google.svg`
#### 使用jsDelivr访问的具体路径为：
```git
https://cdn.jsdelivr.net/gh/GitHub用户名/GitHub仓库@releases版本号/文件在该仓库中的路径
```
