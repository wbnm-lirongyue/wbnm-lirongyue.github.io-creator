---
title: "如何用hugo搭建个人博客"
date: 2020-01-15T20:44:38+08:00
draft: false
---

# 
## 
### 今天用hugo搭建了自己的博客，给大家分享一下过程
主要有以下4个部分
<!--more-->
![2.png](https://i.loli.net/2020/01/15/fWC7ouYVB1IDsya.png)
1. hugo安装
   
   下载hugo_xxx-Windows-64bit.zip,下载网址为：[hugo下载地址](https://github.com/gohugoio/hugo/releases); 我把hugo.exe解压到了D:\Software\hugo\hugo.exe,并把D:\Software\hugo加到了环境变量PATH里,打开VScode,终端运行hugo version查看版本,有版本号则安装成功;
2. vscode终端运行命令行
   
   * cd /d/jirengu
   * hugo new site wbnm-lirongyue.github.io-creator  (wbnm-lirongyue为我的github用户名)
   * cd wbnm-lirongyue.github.io-creator
   * git init
   * git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke  (设置主题，我用的默认主题ananke)
   * echo 'theme = "ananke"' >> config.toml
   * hugo new posts/如何用hugo搭建个人博客.md(文字部分为我的博客标题名)
   * 右边资源管理器content目录中会出现：如何用hugo搭建个人博客.md文件，更改标题，在下面写下你的内容，把draft状态改为false
   * hugo server
   * 右侧资源管理器更改config.toml文件：语言改为zh-Hans，baseURL改为https://wbnm-lirongyue.github.io
   * hugo(重开一个控制台)，此时资源管理器会增加一个public文件夹
   * cd public
   * 新建.gitignore文件夹，将/public/放进去
   * git init
   * git add .
   * gc
  
3. github远程仓库设置

   * 新建仓库，仓库名必须为：wbnm-lirongyue.github.io
   * git remote add origin git@github.com.wbnm-lirongyue.github.io.git
   * git push -u origin master
  
4. 运行网址
   * 浏览器中运行"wbnm-lirongyue.github.io",我的博客就开通啦！

好开心，再接再厉！
![1.png](https://i.loli.net/2020/01/15/zkGOpBNFyLm7gnY.png)

   


