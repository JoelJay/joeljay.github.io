title: Git 中文乱码
date: 2014-01-17 17:27:32
tags: Git
categories: Git
---

1.  ###解决问题的总的思路

    能用Unicode的地方都用Unicode。

2.  ###安装选项 

    - 在 Select Components 中，选定 Use a TrueType font in all console window (not only for Git Bash)
    - 在 Adjusting your PATH environment 中，选定 Run Git from the windows Command Prompt\
    - 其他选项保留缺省值

3. ###解决MSYS bash 中ls 中文显示???问题

    编辑 etc\git-completion.bash，在最后加入

		alias ls='ls --show-control-chars --color=auto'

4. ###解决git status 乱码

		git config --global core.quotepath false

5. ###解决gitk显示文件内容中文乱码

    在%git%\etc\gitconfig文件修改或添加：

		[gui]
		encoding = utf-8

		[i18n]
		commitencoding = {utf-8|gbk}

##注意:
在修改git配置文件的时候保存时出现以下提示：

![save_failed](/img/save_failed.jpg "save_failed")

最终通过另存为一份，再替换掉原来的配置文件保存成功。