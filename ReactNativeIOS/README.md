# react native ios 常见问题
> 欢迎补充

### 0x00a iOS 获取AppStored 中应用的下载地址

一般 苹果的下载地址都是这样

> https://itunes.apple.com/cn/app/id123456789?mt=8

如果你的应用上传了appStore 那么就会分配一个应用id

替换上面链接的 id xxxxx ?mt=8中的xxx就是你的app id

### 0x00b [iOS]解决模拟器无法输入中文问题

第一步：设置schem

>菜单项 －> Product-> Scheme -> Edit Scheme -> 然后在弹出的界面里 选择OPtion 项， 设置 Application Region 为 “中国”

第二步：设置模拟器为中文