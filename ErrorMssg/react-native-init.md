### 0x001
react-native初始化项目时候报错
> Couldn't find package "0.41" on the "npm" registry.
> Command failed: yarn add 0.41 --exact

此错误出现在安装`yarn`之后
#### 解决方案
（1）如果使用`--version`参数创建指定版本的项目，版本号必须精确到两个小数点。

	react-native init MyApp --version 0.39.2。

（2）如果没解决的话请试试：

```cmd
npm config set registry https://registry.npm.taobao.org

```

```cmd
npm config set disturl https://npm.taobao.org/dist

```
（3）请检查是否是网络、代理问题

	