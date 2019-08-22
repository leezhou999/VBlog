2019年8月22日 22:15:32

从git pull下来后，添加了.gitignore，(包含.idea，.iml)

获取了maven依赖

执行了SQL脚本，运行了项目

2019年8月22日 22:24:51

tomcat端口，8081

打包war包，远程部署失败，原因：需要修改pom和配置
https://yq.aliyun.com/articles/479023

1修改pom中打包方式为war

2移除pom中内置tomcat依赖

3添加servletAPI依赖

4修改启动类，重写初始化方法

5war包热部署

2019年8月22日 22:28:49

问题：

war包热部署后，远程项目无法访问

1 解决方案：使用http代替https访问

login页静态资源404

2 解决方案：js，css等相对路径改为 static/js/……
http://www.divcss5.com/html/h50801.shtml

3 **登录后，无法跳转**

原因：mapping相对路径缺少项目名上下文，接收login请求的控制器404





