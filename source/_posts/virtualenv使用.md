title: "virtualenv使用"
id: 25
date: 2011-12-25 04:10:57
tags: 
categories: 
- Uncategorized
---

1\. 从官方页面下载最新版，并解压

地址：[url]http://pypi.python.org/pypi/virtualenv[/url]

2\. 创建自己的虚拟环境：

进入解压后的目录执行：
[code="java"]$ python virtualenv.py ENV[/code]
(如果是安装了virtualenv，可以直接在终端里执行virtualenv ENV)

执行以上后，会创建以下目录：
ENV/lib/pythonX.X/site-packages 激活虚拟环境后，通过pip或easy_install安装的文件都会放置在此
ENV/bin/python 激活虚拟环境后，会使用这里面的python解释器

3\. 激活虚拟环境：
[code="java"]$ source ENV/bin/activate[/code]

4\. 退出虚拟环境：
[code="java"]$ deactivate[/code]

&nbsp;