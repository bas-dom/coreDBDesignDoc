# 智慧运维工作站软件(OM-Site)开发详细文档 #

## 软件背景 ##

OM是基于工作站组态软件(OM-SiteLab)描绘的组态画面，呈现于项目现场工作站电脑中，并提供用户操作设备、查看运行状态、接受实时报警和交互的一套软件解决方案。

该软件运行于 **windows平台(win7/win10 32位/64位兼容)** 下，一般发布版本为绿色版本，可直接解压运行。

需 **与OM-SiteLab配合使用** ，控制服务器端软件需配套使用 CoreEngine/ LogicEngine两个控制引擎软件。

## 详细设计概述 ##

OM-Site经过概要设计评估，选用React+redux+antd Design+webpack库作为底层构架。

后台使用python Flask Restful API框架，生产环境中采用gunicorn + nginx优化并发性能。

经过详细规划后，系统代码模块分为以下部分：

1. common公共库

2. pages页面分组

3. 每个page分组下分为：
    container：页面控制模块分组
    component：页面控件元素分组
    module：页面逻辑代码分组
    index.js: 入口