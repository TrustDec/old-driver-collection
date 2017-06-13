# Windows 常见问题
> 欢迎补充

#### Windows中删除路径太长目录及文件

> [原文地址](https://stackoverflow.com/questions/551072/how-to-delete-a-long-path-in-windows)

> 主要执行：

- 新建空白目录

- 管理员方式打开命令行窗口；

- 输入```robocopy D:\xxx\temp D:\xxx\test\node_modules /purge```


```console
	robocopy (新建的空白目录) (要删除的目录) /purge
```

> 此方法将删除目标路径下所有文件，慎用！！！
