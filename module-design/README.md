# 模块设计

本项目采用**React+redux+antd Design+webpack**等搭建开发环境，以及其他一些第三方库。

由于react的state只能管理自己内部组件的状态，props是只能从父级组件向子组件单向分发的单向数据流，更多时候，我们需要组件之间的互相联系，所以项目中React只负责功能模块的组件化，然后使用Redux来管理状态，使用**connect将react组件和redux连接在一起**。

通过action提供事件发生的要素，reducer捕捉到与自己匹配的action，进行逻辑处理，修改store中的状态，然后通过Provider组件作为顶层组件，将store分发给所有被connect的组件。

**Ant Design**提供一些通用的UI组件。

**webpack**对项目进行打包。
