title: Hexo 博客中插入视频
date: 2014-03-13 10:17:41
tags: Hexo
categories: Hexo
---

Hexo 博客的文章都是用Markdown语法来完成。不过对于视频需求Markdown语法里没有涉及到，只能另辟蹊径。

注意到Markdown里可以嵌入Html代码段混合编写文章。于是有了如下两种解决方案：

1. 使用Video 标签

	~~~html
	<video id="video1" controls="" preload="none" poster="img/ISO.png">
	  <source id="mp4" src="http://f.youku.com/player/getFlvPath/sid/139461078077272_01/st/mp4/fileid/030008010051319E0B684A059066D930A5B744-FFDB-2034-2EAC-7F5451FC4B45?K=f2fb3ec1952cb57c282960bf&hd=1&ts=124&ctype=40" type="video/mp4">
	  <p>Your user agent does not support the HTML5 Video element. 
		See original link:http://v.youku.com/v_show/id_XNTIxMjU2NTUy.html </p>
	</video>   
	~~~

	其中source中src是通过工具抓取到的优酷视频真实的地址, 不过这个地址会经常变动，会出现视频不能播放的情况。
	src也可以把我们要播放的视频上传到服务端，一般视频都比较大很耗资源，不太建议这种做法。

2. 使用embed标签<strong><font color="red">（推荐）</font></strong> 

	~~~html
	<object width="672" height="378">
	  <param name="movie" value="http://player.youku.com/player.php/sid/XNTIxMjU2NTUy/v.swf"></param>
	  <param name="allowFullScreen" value="true"></param>
	  <param name="allowscriptaccess" value="always"></param>
	  <embed src="http://player.youku.com/player.php/sid/XNTIxMjU2NTUy/v.swf"
		type="application/x-shockwave-flash" allowscriptaccess="always" allowfullscreen="true"
		width="672" height="378">
	  </embed>
	</object>
	~~~
	
	这里embed标签的src是优酷分享时提供的swf地址，这个地址获取比较方便。就只有会有广告出现的缺点，这也无伤大雅。

此文仅以优酷视频为例，其他类型类比之。