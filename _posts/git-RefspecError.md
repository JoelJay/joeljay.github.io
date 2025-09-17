title: Git error Refspec master matches more than one
date: 2015-01-30 17:33:48
tags: Git
---

写完代码commit之后，通过Android Studio的集成git工具想要Push代码到远程仓库。
结果发现刚刚commit的代码未出现在Push列表里，列表空空如也。倍感疑惑，既然继承工具不能成功。

只好使用Git 命令去push，但是出现了如下的错误：

	$ git push origin master
	error: src refspec master matches more than one.
	fatal: Authentication failed for 'host/liangjie/someproject.git'

经过一段时间的摸索，终于发现了问题所在：

	$ git tag
	6.0test
	master


由于某个小伙伴创建了一个用来测试的master tag，所以出现了"Refspec master matches more than one"。

解决方式很简单，删除这个用于测试的master tag(-__-)b就可以了。

	$ git tag -d master
	Deleted tag 'master' (was 138c31a)

Notice: 打tag的时候名称最好不要同分支名称一致，否则就会出现上诉错误。