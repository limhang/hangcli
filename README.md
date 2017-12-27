# hangcli

[![PyPI version](https://badge.fury.io/py/hangcli.svg)](https://badge.fury.io/py/hangcli)

基于python3.x的脚手架工具，方便构建应用，目前支持react项目

---

## 一、使用
### 1-1、初始化hangcli到本地
```
sudo pip3 install hangcli
```

### 1-2、构建react应用
在终端执行
```
hangcli react --project=yourprojectname
```

## 二、脚手架详细介绍
### 2-1、工程结构
```
|____hangcli.py
|____setup.py
|____src
| |____react
| | |____.babelrc
| | |____index.html
| | |____index.js
| | |____package.json
| | |____webpack.config.js
|____upload.py
```
目前的功能较少，所以结构也很简单
其中`hangcli.py`实现主要cli功能，`setup.py`指定打包pypi配置信息，`upload.py`是上架打包脚本，`src/react`中存放react项目需要用的文件。

### 2-2、打包到pypi操作
修改了脚手架代码之后，我们首先需要更新`setup.py`中的版本信息，然后执行`upload.py`脚本之后，输入用户名和密码。


### 2-3、关于react应用构建
#### 2-3-1、目前支持的功能
* configured webpack.config.js && package.json
* less && scss loader in box
* include spread function

## 三、参考文档
[upload your package into pypi](https://stackoverflow.com/questions/45207128/failed-to-upload-packages-to-pypi-410-gone
)

[detail info about load your package into pypi](https://hk.saowen.com/a/04174ec24587c9b38c6f4c945ebffacf40f7ff835c70429cf71b40bc3edc3470
)


