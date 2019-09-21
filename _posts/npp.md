---
layout: post
title:  "npp"
categories: Other
tags: Other
author: joshua
description: notepad++
---

[notepad++如何更改编辑界面前背景颜色](https://jingyan.baidu.com/article/5552ef47e7178f518ffbc9d1.html)
- 【设置】-【语言格式设置...】 - 【Global Styles】-【Default Style】

[notePad++修改颜色](http://javanotestxt.iteye.com/blog/2268464)
- Notepad++的配置全部使用xml文件来保存，其中配色方案保存在stylers.xml，这个文件就位于notepad安装文件的根目录

  #### Global Styles

	Indent guideline style  缩进参考线的颜色
	Brace highlight style   鼠标指针在框架左右时框架的颜色（如css中{}   js中的（））
	Bad brace color         错误的框架的颜色（如js中{}里面有错误，这个{}的颜色）
	Current line background colour  鼠标指向的当前行的背景颜色
	Selected text colour    选中文本的颜色
	Caret colour            鼠标指针的颜色
	Line number margin      行号数字的颜色
	Fold                    隐藏代码按钮颜色
	Fold margin             隐藏代码按钮上下背景颜色
	Smart HighLighting      双击选择文字的背景颜色
	Tags match highlighting 鼠标指针在当前标签时该标签的背景颜色
	Tags attribute          鼠标指针在当前标签时属性和属性值的背景颜色
	Active tab focused      出现连个文档界面时选中的文档的背景颜色
	Active tab unfocused    出现连个文档界面时没选中的文档的背景颜色（另一视图的第一个文档）
	Active tab text         当前文档的名称的颜色
	Inactive tabs           未选中的文档的标签背景颜色


https://notepad-plus-plus.org/repository/7.x/7.5.8/npp.7.5.8.sha1.md5.digest.txt
- SHA-1
  - feda36051199971832b0c822e30b6f7fda5894f9    npp.7.5.8.Installer.exe
  - 19a9a168e523637b56cb15afad6377f09f3cb6aa    npp.7.5.8.Installer.x64.exe
- md5
  - 077268086e3e4dba46b1bd1ee1ef521c  npp.7.5.8.Installer.exe
  - 538431fd315f4da79eefc9072e4146a8  npp.7.5.8.Installer.x64.exe



### [实用技巧](https://blog.csdn.net/so_geili/article/details/79317001)
- 在7.5之前的版本中，32bit版有插件管理功能，64bit版没有插件管理功能。
- 在7.5之后的版本中，无论32bit还是64bit版，都没有插件管理功能了。
- Don’t use %APPDATA% 
默认没勾选。作用是允许配置文件放在Notepad++的安装路径下。由此，可以实现支持把整个Notepad++根目录都放到U盘中，到处带着跑了。当使用者对于Notepad++有很多自定义的配置，而换了个电脑，就得重新配置Notepad++时，建议勾选该选项。
- Allow plugins to be loaded from %APPDATA%\notepad++\plugins 
默认没勾选。作用是允许从%APPDATA%\notepad++\plugins的位置，载入插件，有一定的安全隐患。因为有些不安全的插件，如果放到plugins目录下的话，其也会自动载入

  - [github上32&64bit的PluginManager下载地址](https://github.com/bruderstein/nppPluginManager/releases)
  - [csdn上32bit的PluginManager_v1.4.9_UNI .7z下载地址](http://download.csdn.net/download/so_geili/10250811)
  - [csdn上64bit的PluginManager_v1.4.9_x64.7z下载地址](http://download.csdn.net/download/so_geili/10250819)

plugins文件夹下的PluginManager.dll

[插件的官方网站](http://sourceforge.net/projects/npp-plugins/files/)
```
    添加书签 	CTRL+F2 或 直接鼠标右击左侧栏(和设置断点类似)
    快速定位书签 	F2
    快速复制一行	  CTRL+D
    快速删除一行	  CTRL+L
    将上下行交换	  CTRL+T
    快速定位到某一行	  CTRL+G
    快速查询	  CTRL+F
    进行单行注释	  CTRL+K 或者是 CTRL+Q
    取消单行注释	  CTRL+SHIFT+K 或者是 CTRL+Q
    进行多行注释	  CTRL+SHIFT+Q
    字体放大、缩小	  点击放大、缩小按钮 或  CTRL+鼠标+滚轮的方式
    选择多行	  鼠标右击出现： “开始/结束” 最后一行选择 “开始/结束”
    折叠所有行	  ALT+0
    释放所有行	  ALT+SHIFT+0
    折叠当前行	  CTRL+ALT+F
    释放当前行	  CTRL+ALT+SHIFT+F
    全屏模式	  F11     (和浏览器一样)
    合并行	  Ctrl+J

四、 设置tab键
    设置 ->首选项… ->选项卡设置
六、 自动补全
    设置 -> 首选项 -> 自动完成
Json Viewer插件格式化数据
json数据作为实参，用一行代码显示
    移除行首行尾空格，合并行
```


[Notepad2-mod](https://www.cnblogs.com/best/p/5819858.html)
- Notepad2 的修改版、更新很及时，支持代码折叠、NSIS、Inno、AHK语法高亮等
- http://xhmikosr.io/notepad2-mod/
- https://github.com/XhmikosR/notepad2-mod
- 中文绿色色版下载 http://www.cr173.com/soft/6498.html


[删除XML代码注释](https://jingyan.baidu.com/article/c275f6ba08647ae33d756796.html)
```
ctrl+f
<!-[\s\S]*?->
正则
全部替换
```


[删除空白行](http://blog.csdn.net/q277055799/article/details/19408417)
1. 先下载安装插件 TextFX，下载后重新启动下，然后在菜单栏找到 TextFX -> TextFX Edit -> Delete blank lines，即可
2. 选择替换，把查找模式设置为正则表达式，在查找框中输入 ^\s+  ,替换框留空，点"全部替换"，即可(先全选)
3. 删除空行(不包括有空格类符号的空行)
4. \r\n转义符替换

   按ctrl+h，跳出搜索替换框，把查找模式定义为扩展(\n，\r…)
   查找目标：\r\n\r\n
   替换为：\r\n

   

[快捷键](https://www.cnblogs.com/jungege/p/6003992.html)

```
Ctrl-T          复制当前行至剪贴板（注：帮助中说是将当前行与上一行交换位置）
Ctrl-Shift-Up	将当前行上移一行
Ctrl-Shift-Down	将当前行下移一行
Ctrl-L          删除当前行
ALT-C           列编辑器
Ctrl-Q          添加/删除注释
Ctrl-Shift-Q	区块添加/删除注释
Ctrl-G          跳转至某行对话框
```
[列编辑](https://www.cnblogs.com/jpfss/p/9353203.html)
- 插入数字

[添加或删除不连续的列](https://blog.csdn.net/zhoukun1314/article/details/82719076)
- 设置—首选项—编辑，可以选择多列编辑，启动ctrl+鼠标点选，就可以进行多列不连续的编辑了
