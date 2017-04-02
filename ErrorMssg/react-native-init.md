### 0x001： react-native初始化项目时候报错

> Couldn't find package "xxx" on the "npm" registry.
> Command failed: yarn add xxx --exact

提示在npm仓库里没有xxx的版本

#### 解决方案
（1）如果使用`--version`参数创建指定版本的项目，版本号必须精确到两个小数点。
```cmd
react-native init MyApp --version 0.39.2。
```
（2）如果没解决的话请试试：

```cmd
npm config set registry https://registry.npm.taobao.org

```

```cmd
npm config set disturl https://npm.taobao.org/dist

```

	