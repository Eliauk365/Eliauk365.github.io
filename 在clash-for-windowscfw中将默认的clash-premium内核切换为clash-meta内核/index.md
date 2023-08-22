# 在Clash for Windows（CFW）中将默认的Clash Premium内核切换为Clash Meta内核


> 文章转载于：https://blog.misaka.rest/2023/04/19/cfw-change-meta/

在我们使用Clash For Windows（以下均使用CFW指代）时，有时候需要使用Clash Meta内核。对于习惯CFW的用户来说，切换客户端有时是一件忍痛割爱的事情。那在这篇教程中，我来和大家一起来在CFW中将默认的Clash Premium内核切换为Clash Meta内核。

准备材料
Clash For Windows
部署步骤
打开 Clash Meta 的项目下载地址：https://github.com/MetaCubeX/Clash.Meta/releases ，下载适合自己电脑的版本
![](https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230419102506.png)

解压内核程序，备用
![](https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230419102541.png)

进入CFW的安装目录中的resources/static/files/win/x64（如为32位系统的程序则为x86），将默认的clash-win64.exe更名备份，我这里就改为clash-win642.exe
将第二步解压的内核程序复制进来，并改为clash-win64.exe
![](https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230419102813.png)

打开CFW，当此处出现“Unknown”即为切换成功
![](https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230419102849.png)
