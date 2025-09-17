title: Hexo spawn ENOENT
date: 2014-01-17 17:27:32
tags: Hexo
categories: Hexo
---


在使用hexo deploy命令时，出现了以下错误：

```sh
Clearing
Copying files from public folder.
events.js:72
        throw er; // Unhandled 'error' event
              ^
Error: spawn ENOENT
    at errnoException (child_process.js:980:11)
    at Process.ChildProcess._handle.onexit (child_process.js:771:34)
```

解决方法：在cmd下敲hexo命令会有问题，在git shell下面敲使用命令就可以了。
