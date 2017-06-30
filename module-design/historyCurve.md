# 历史曲线模块

历史曲线模块一共分为 `ChartView.js` 、`ConfigModalView.js`、`PointListView.js` 、`HistoryView.js`  4个组件。 分别代表了历史曲线的历史曲线显示页面、配置规则窗口、选取项目中所有点位的窗口和结合其他三个组件的父组件。

`HistoryView.js`作为父组件，将数据分发给子组件。`ChartView.js`使用`echarts-for-react`库，将选择的点位在一段时间内的点值通过图标的形式显示出来。`ConfigModalView.js`是一个配置逻辑的组件，程序根据你输入的时间范围，间隔时间生成不同的图表。`PointListView.js`这个组件主要显示项目中的点位，可供用户筛选点位。

