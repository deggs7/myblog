title: "python包管理整理"
id: 28
date: 2011-11-03 08:30:38
tags: 
categories: 
- Uncategorized
---

easy_insall的作用和perl中的cpan, ruby中的gem类似，都提供了在线一键安装模块的傻瓜方便方式
pip是easy_install的改进版, 提供更好的提示信息，删除package等功能。（老版本的python中只有easy_install, 没有pip）

easy_install的用法：

1） 安装一个包
$ easy_install &lt;package_name&gt;
$ easy_install "&lt;package_name&gt;==&lt;version&gt;"

2) 升级一个包
$ easy_install -U "&lt;package_name&gt;&gt;=&lt;version&gt;"

pip的用法

1) 安装一个包
$ pip install &lt;package_name&gt;
$ pip install &lt;package_name&gt;==&lt;version&gt;

2) 升级一个包 (如果不提供version号，升级到最新版本）
$ pip install --upgrade &lt;package_name&gt;&gt;=&lt;version&gt;

3）删除一个包
$ pip uninstall &lt;package_name&gt;