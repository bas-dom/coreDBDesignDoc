# 用户管理模块

用户管理模块包含了管理用户和切换用户两个组件。

### 1. 管理用户组件
该组件使用`UserManagerModal`作为父组件，通过UserAddModal对用户进行增加，通过`UserModifyModal`对用户进行修改，通过`ValueList`对用户进行删除。

### 2. 切换用户组件
该组件使用SwitchUser作为父组件，用SwitchUserFormView里的Form表单向后台提交用户名及密码，使用方法同登录模块。