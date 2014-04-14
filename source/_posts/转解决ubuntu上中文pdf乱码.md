title: "解决ubuntu上中文pdf乱码"
id: 26
date: 2011-12-10 01:19:18
tags: 
categories: 
- Uncategorized
---

Ubuntu自带的Document Viewer支持pdf文件，但是打开中文pdf文件时，会出现乱码。

解决办法：

1.下载poppler-data（[http://poppler.freedesktop.org/poppler-data-0.1.tar.gz](http://poppler.freedesktop.org/poppler-data-0.1.tar.gz)），解压
2.在终端执行：cd /解压路径/poppler-data-0.1
3.再输入：sudo make install datadir=/usr/share