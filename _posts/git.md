title: Git多账号切换
date: 2014-03-06 10:21:59
tags: Git
categories: Git
---

有时候会遇到需要使用多个git账号的情况，手动切换是在过于麻烦。

于是就有了一下的解决方案：

首先，切换到ssh的key目录下：
	
	cd ~/.ssh

然后使用ssh-keygen命令创建一个新的SSH key:
	
	ssh-keygen -t rsa -C  "sencond@mail.com" -f id_rsa_second

其中id_rsa_second表示保存的key的名称,可以自定义，命令执行之后会在.ssh目录里出现两个文件其中id_rsa_second.pub表示公钥。后面会用到。

由于默认情况下，每次进行SSH连接时默认发送本地钥匙（默认为~/.ssh/id_rsa）。所以之前生成的id_rsa_second在默认情况下是没有被用到的。

这时就需要在~/.ssh 目录创建config文件，该文件用于配置钥匙对应的服务器信息。具体语法如下：

	Host    别名
		HostName        主机名
		Port            端口
		User            用户名
		IdentityFile    密钥文件的路径

其中Host别名自己任意给出，能方便记忆就行。给出一个示例配置以供参考：

	# Default github user(first@mail.com)
	Host github.com
		 HostName github.com
		 User git
		 IdentityFile ~/.ssh/id_rsa

	# second user(second@mail.com)
	Host github-second
		 HostName github.com
		 User git
		 IdentityFile ~/.ssh/id_rsa_second
		 
配置完成之后，在连接非默认账号需要修改一下远程库的地址，
如本来的远程库地址为git@github:sencond/test.git
现在就需要改为git@github-second:sencond/test.git。

而且通过 ssh + 别名就能登录远程库

####注意：
1. 切换账号的时候要修改相应的配置文件
		git config --global user.name 用户名
		git config --global user.email second@email.com

2. 在远程端添加前面生成的id_rsa_second.pub的公钥到远程库里。
	
3. 使用对应的ssh key密码。


###Enjoy it!