# 用户登录模块

用户登录模块使用`LoginForm`和`ConfigModal`组件，通过`Form`表单向接口`/login`传送用户输入的用户名和密码，通过`toggleIsRememeber`方法判断是否记住密码，若记住则保存到`localStorage`中，下次可以通过`getInitLoginInfo`查看浏览器是否存有用户信息。