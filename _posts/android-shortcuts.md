title: Android Studio 常用快捷总结
date: 2015-01-22 11:17:48
tags: Android
categories: Android
---

最近又开始Android Develop了。不过Google发布了Android Studio开发工具，终于可以不用臃肿的Eclipse。大快人心啊！

记录一下在工作经常使用到的快捷键操作:

### 调试
	- F5 	进入函数内
	- F6 	单步跟踪
	- F7 	由函数内部返回至调用处
	- F8 	继续执行直到下个断点


### 注释
	- CTRL + /                  注释选中代码以“//...”格式
	- CTRL + SHIFT + /          注释选中代码以“/*...*/”格式
	- ALT + SHIFT + J           添加文件，方法，属性的注释
	- CTRL + SHIFT + ‘-’        折叠代码
	- CTRL + Shift + ‘+’        打开折叠代码


### 代码生成
	- CTRL + I                  Implement methods
	- CTRL + O                  Override methods
	- ALT + Insert              打开Generate菜单


### 查找
	- CTRL + F + (SHIFT)        查找（全局）
	- CTRL + R + (SHIFT)        替换（全局）
	- CTRL + H                  高级查找
	- Double SHIFT              搜索所有地方
	- CTRL + N                  搜索类名
	- CTRL + SHIFT + F7         搜索选中的文本


### 导航打开
	- CTRL + F12                文件大纲视图
	- CTRL + E                  打开近期的文件
	- SHIFT + F4                新窗口打开 
	- CTRL + ALT + 左箭头        导航到上一步
	- CTRL + ALT + 右箭头        导航到下一步
	- CTRL + G                  跳转到指定行


### 编辑
	- CTRL + D                  复制整行
	- SHIFT + ENTER             开辟新行
	- CTRL + SHIFT + U          大小写切换
	- CTRL + SHIFT + Up/Down    上下行切换


### 重构
	- SHIFT + F6                重命名方法
	- CTRL + F6                 修改方法签名
	- CTRL + SHIFT + L          格式化代码
	- CTRL + ALT + O            整理Import
	- F5                        复制类
	- F6                        移动类
