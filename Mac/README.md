# Mac 常见问题
> 欢迎补充

### 0x00a Mac笔记本无法加入wifi网络
> [Mac笔记本无法加入wifi网络](https://www.zhihu.com/question/20026105)

### 0x00b Mac自带的本地服务器的使用
> [Mac自带的本地服务器的使用](Mac自带的本地服务器的使用)

- 开启apache:  ```sudo apachectl start```

- 重启apache:  ```sudo apachectl restart```

- 关闭apache:  ```sudo apachectl stop```

> 回车会提示输入密码，也就是你电脑的密码，http://127.0.0.1/测试一下

> 点击Finder,然后Command+Shift+G,前往```/Library/WebServer/Documents```

默认打开的是index.html.en

> 如果没有正常显示，提示说没有权限时，单击该文件，然后Command+I在末尾设置权限即可。

> 使用过后，记得关闭服务器，要不然会一直消耗你电脑内存，后果你懂的。

