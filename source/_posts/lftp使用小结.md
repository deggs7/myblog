title: "lftp使用小结"
id: 29
date: 2011-10-23 02:53:53
tags: 
categories: 
- Uncategorized
---

<div id="blog_content">lftp基本使用

[登陆]

登陆：lftp ftp://user@site
输入密码
（其他方式，为明文密码
lftp ftp://user:password@site:port
lftp user:password@site:port
lftp site -p port -u user,password
lftp site:port -u user,password ）

[登陆后对远端的操作]

ls
查看远端文件列表

cd
进入远端目录

get/put
获得／上传文件

mget/mput
获得／上传文件（可以使用通配符）

mirror/(mirror -R)
获得／上传整个文件夹

pget
多线程下载文件（默认是5个）

rm
删除远端文件

mrm
删除多个远端文件（使用同配符）

mv
移动或者重命名远端文件

mkdir
创建远端文件夹

rmdir
删除远端文件夹

du
查看远端文件大小

lpwd
查看本地当前文件夹

lcd
切换本地当前文件夹

[bookmark使用]

bookmark
支持下面的子命令:

add &lt;name&gt; [&lt;loc&gt;]
把当前位置或指定的位置加入书签,并使用给定名字

del &lt;name&gt;
删除指定名字的书签

edit
编辑书签文件

import &lt;type&gt;
导入其他程序的书签

list
列出书签 (默认)

[其他问题]

问题：
乱码：通常ftp服务器的编码是gbk，而linux主机默认是utf-8，所以访问ftp时看到的都是乱码。
解决：
设置ftp编码：  set ftp:charset gbk
设置本机编码：set file:charset utf-8
永久解决
编辑文件（如果没有则建立）~/.lftp/rc , 输入下面两行：
set ftp:charset gbk
set file:charset utf8</div>
&nbsp;
<div id="bottoms"></div>