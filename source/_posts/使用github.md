title: "使用github"
id: 31
date: 2011-08-06 09:32:25
tags: 
categories: 
- Uncategorized
---

学习使用github，基本理解了Git的原理
记录一下过程，留做备忘

**1.安装好git后，需要针对github的设置：**

$ git config --global user.name "Firstname Lastname"
The name should be your actual name, not your GitHub username.
Sets the name of the user for all git instances on the system

$ git config --global user.email "your_email@youremail.com"
Sets the email of the user for all git instances on the system

$ git config --global github.user username
Sets the GitHub username for all git instances on the system

$ git config --global github.token 0123456789yourf0123456789token
Sets the GitHub token for all git instances on the system

$ git config --list 可以查看config的所有配置项

详细过程：http://help.github.com/linux-set-up-git/

**2.新建Repository**

在github中新建一个repository,记住名字

$ mkdir ~/Hello-World
Creates a directory for your project called "Hello-World" in your user directory

$ cd ~/Hello-World
Changes the current working directory to your newly created directory

$ git init
Sets up the necessary Git files

$ touch README

本地提交

$ git add README
Stages your README file, adding it to the list of files to be committed

$ git commit -m 'first commit'

**管理远程仓储库**

真正放入github中

$ git remote add origin git@github.com:username/Hello-World.git
Sets the origin for the Hello-World repo

$ git push origin master

要查看当前配置有哪些远程仓库，可以用 git remote 命令，它会列出每个远程库的简短名字。在克隆完某个项目后，至少可以看到一个名为 origin 的远程库，Git 默认使用这个名字来标识你所克隆的原始仓库

详细：http://help.github.com/create-a-repo/

一些关于git的教程：

http://www.linuxsir.org/main/doc/git/gittutorcn.htm

http://progit.org/book/zh/ch2-5.html

http://neverloser.iteye.com/blog/1090244