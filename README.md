## react-native-common-problems

本项目的主旨是为了找出`react-native`开发中常遇到的问题，并寻找解决办法。

### JS

### iOS

- 在不修改`info.plist`文件之前，一定要用`https`的网络请求(如何修改请百度)，或以如下方式配置：

  ### ![iOS_Plist_Http](https://github.com/mah93/react-native-common-problems/blob/master/image/iOS_Plist_Http.png)

- 在使用定位，拍照，相机等权限的时候，需要在`info.plist`中做出修改
- 搜索框、长按等出来的菜单，做本地化处理后，可显示中文
- 在RN0.45版本后，iOS新建项目之前需要配置`third-party`，请按照下面教程操作[iOS RN 0.45以上版本所需的第三方编译库(boost等)](https://reactnative.cn/post/4301)

### Android

- 真机调试的时候，需要在`Dev Settings`里面修改`Debug server host & port for device`，将`本地IP + :8081`填入输入框
- 真机调试的时候，如果无法通过摇一摇唤起开发菜单，可以通过终端运行`adb shell input keyevent 82`唤起
- 真机调试的时候，小米、魅族要开启悬浮窗权限和关闭MIUI优化

### 通用

- 0.52版本`react-native-vector-icons`正常安装后不能使用。

  解决方式：执行`rm ./node_modules/react-native/local-cli/core/__fixtures__/files/package.json`

  参考[https://github.com/oblador/react-native-vector-icons/issues/626](https://github.com/oblador/react-native-vector-icons/issues/626)

### 环境

### 版本

### 布局
