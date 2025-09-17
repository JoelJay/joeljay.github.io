title: Android调试logcat 不输出信息
date: 2014-02-10 16:45:03
tags: [Android, Eclipse]
categories: Android
---

重启adb，如果使用eclipse，先关闭eclipse，再重启adb，再启动eclipse

```sh
adb kill-server
adb start-server
```
Done!