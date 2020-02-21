---
layout: post
title: "完全卸载mysql"
date: 2020-2-19
categories: install && unstall
---
win+s->在搜索中输入control->回车进入控制面板->找到卸载程序

<figure>
	<a><img src="{{site.url}}/pics/control1.png"></a>
</figure>

将那些带mysql的全部卸载

打开C:\Program Files找到MySQL文件夹ctrl+d删除

打开C:\ProgramData找到MySQL文件夹ctrl+d删除

win+r 输入regedit打开注册表目录`HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Services\MySQL80`删除MySQL80文件夹

重新打开mysqlinstaller进行安装