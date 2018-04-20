# Android 常见问题
> 欢迎补充

### 0x00a Android Studio 创建项目卡在 `Building "project name" Gradle project info`

> 原因:由网络原因,Gradle下载不了or速度慢，导致无法打开新建项目
#### 解决方案 离线安装

下载匹配版本 [点击进入下载地址](https://services.gradle.org/distributions/)

问题1: 并不知道AS创建新项目时下载的`gradle`版本号？

> 解决方式一：

打开活动监视器->点击网络->查找AS进程->双击进程->点击打开文件和端口-滑动到最底部->[`command+f`]关键字搜索gradle->即可看到`gradle-x.x(.x)-all-zip`

> 解决方式一：

进入访达 -> [`command+shift+.`]显示隐藏文件 -> 找到`.gradle`->进入`.gradle/wrapper/dists/gradle-x-x-x-all/(串码)` ->可确定AS当前下载的版本(AS一般默认下载最新的gradle)

下载完成之后，放入`.gradle/wrapper/dists/gradle-x-x-x-all/(串码)`下双击解压

然后重新打开AS创建项目

PS：AS 3.0.1成功创建项目后报一些错误，Google查找许久未解决，后来将AS版本更新为3.1.1后,重新创建项目自动下载`gradle-4.4-all`、其他相关包依赖,一切顺利

3.0.1创建项目后报错(部分报错)
 - Failed to resolve: junit:junit:4.12 ( 网上为了回避问题删除testImplementation 'junit:junit:4.12'，简直无语😓)
 - Could not resolve com.android.support:appcompat-v7:26.1.0 [duplicate]
 - Could not resolve com.android.support.constraint:constraint-layout:1.1.0
 - Could not resolve com.android.support.test.espresso:espresso-core:3.0.1

