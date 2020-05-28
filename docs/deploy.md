# 部署

## 部署

如果您希望部署深科技的LBS的“Web前端”到您自己的服务器上，步骤如下：



### 安装node.js

安装包下载及详细安装说明参考nodejs官网:

```console
https://nodejs.org/zh-cn/download
```

### 下载源代码

```console
$ git clone https://github.com/kaifapdc/lbs-web.git
```

### 安装
命令行模式，进入克隆的前端代码库根目录，运行下述指令安装依赖包
```console
$ npm install
```

命令行模式，运行下述指令，启动运行前端应用web服务
```console
$ npm start
```

### 访问
安装完成后，在浏览器中键入以下URL即可访问LBS应用
```console
http://ip-address:8000/monitor
```

## 二次开发

如果您想集成深科技的LBS平台，进行二次开发，

请参考我们的[开源代码](https://github.com/kaifapdc/lbs-web/)，以及[学习API](./api.md)。

我们的“后端服务器”，与我们的定位终端通讯，为“Web前段”提供数据等繁琐的工作。

您只需聚焦在您业务逻辑上，修改Web前段，这样大大加快了开发速度。



名字                               | 开源 | 细节
---------------------------------- | -------- | -------
Web前端 | 是      | 前端代码主要负责界面展示和用户交互。
后端服务器 | 否       | 后端代码负责业务逻辑。


{==
此处建议附图为用户解释说明 “系统架构”
请 刘兴平 提供
==}


![Drag Racing](../assets/images/illustration.png)

## 购买套件

如果您打算进行二次开发，而且需要“硬件”来发送数据至服务器，例如：

* 蓝牙定位标签
* 定位微基站
* LoRa网关

您可以[联系我们](./contact.md)购买和获取技术支持
