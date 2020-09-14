# gmall-admin

本项目骇客湾商城管理界面

## 项目搭建

```bash
# Clone project
git clone https://github.com/lisang1995/gmall-admin.git

# Install dependencies
npm install

# 建议不要用cnpm  安装有各种诡异的bug 可以通过如下操作解决npm速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# Server with hot reload at localhost:8888
npm run dev

# Build for production with minification
npm run build

# Build for production and view the bundle analyzer report
npm run build --report
```

### npm install 报错解决

安装python 27环境

npm install 时报错：MSBUILD : error MSB4132: 无法识别工具版本“2.0”。可用的工具版本为 "4.0"。

![](https://img-blog.csdnimg.cn/20191015151701637.png)

解决方法：

1. 从https://download.microsoft.com/download/5/f/7/5f7acaeb-8363-451f-9425-68a90f98b238/visualcppbuildtools_full.exe地址下载Microsoft Visual C++ Build Tools 2015， 选择对应版本的SDK

   ![]( https://img-blog.csdnimg.cn/20191015151859416.png )

2. npm config set msvs_version 2015 --global ，重新执行npm install（如果报错，重新安装node-sass即可）

