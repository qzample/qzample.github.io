---
layout: post
title: 安装完xampp如何配置WordPress
date: 2020-02-21
categories: install && unstall
---

[修改xampp端口号][port]

如果你成功安装好xampp，启动Apache，进入`127.0.0.1:端口号`，看到如下页面：
<figure>
	<a><img src="{{site.url}}/pics/xampp-welcome.png"></a>
</figure>

接着你点击phpMyAdmin，之后会跳转到登录界面，输入mysql的用户名和密码

[xampp下配置mysql用户名和密码][config-mysql]

然后你就会进入到后台数据库界面

<figure>
	<a><img src="{{site.url}}/pics/xampp2.png"></a>
</figure>

我们将下载好的wordpress解压到你的`xampp`安装目录下的htdocs中

回到刚才的后台数据库界面，点击新建，输入你的数据库名称为`WordPress`；

接着打开`wordpress`文件夹下的`wp-config-sample` ，配置好你的`MySQL`数据库名称、账号以及密码

<figure>
	<a><img src="{{site.url}}/pics/wp-config-sample.png"></a>
</figure>

该文件被安装程序用来自动生成wp-config.php配置文件。

访问`127.0.0.1:你的端口号/wordpress`，一步步配置我想不用赘述，只要将你创建的数据库名称密码等填写无误就ok

最后结果

<figure>
	<a><img src="{{site.url}}/pics/wordpress-home.png"></a>
</figure>

[port]: {{site.url}}/install/&&/unstall/2020/02/19/xampp.html#port
[config-mysql]: {{site.url}}/install/&&/unstall/2020/02/19/xampp.html#mysql-config