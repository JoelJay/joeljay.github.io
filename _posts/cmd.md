title: Windows 使用过的cmd命令
date: 2014-03-11 14:38:00
tags: 
categories: Tools
---

#持续更新,先占坑

记录一下用到过的CMD命令

*	cd 命令

	~~~shell
	cd foldername		进入foldername目录			
	cd /d path 		进入具体目录
	cd \			进入根目录
	cd ..			返回上级目录
	~~~
	
*	ipconfig命令
	
	~~~shell
	ipconfig 		IP 配置信息显示IP地址、子网掩码和缺省网关值
	ipconfig /all		显示本机TCP/IP配置详细信息
	~~~

*	文件操作命令
	
	~~~shell
	- 创建目录
	mkdir [drive:] path
	md [drive:] path
	chdir path		进入子目录path
	  
	move  移动文件
	type  显示文件内容（可创建文件）
	type  可用于合并文件内容： type *.txt > all.txt
	~~~

对于各命令的其他可选项通过 /? 查看帮助文档即可