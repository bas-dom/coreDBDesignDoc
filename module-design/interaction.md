# 用户交互模块

用户交互模块包含了控制参数设置、设备详情两个模态框。

### 1. 控制参数设置模态框
控制参数设备组件通过调用`/get_realtimedata`接口内的数据，通过canvas将数据绘制到页面上。页面在打开后会调用`observer.worker.js`中的requestData方法，会每2秒中刷新一次数据，如果数据变动，页面数据就会刷新。并且使用HTML5的webWorker方法实现两个线程件的通讯。通过postMessage将`/get_realtimedata`接口中的数据发送到observerScreen.js中的ObserverScreen类中实现数据的更新，并且改变视图。然后在修改值的时候调用`/common/checkWorker.js`中的`CheckWorker`类实现没两秒中检查一次值是否修改的逻辑。

### 2. 

