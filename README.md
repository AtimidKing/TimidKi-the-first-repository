# TimidKi-the-first-repository
This is one of my learning libraries built using Github
# 创建hello world
## IDE：**eclipse Javaee**
步骤：
1. [下载Struts2的jar包](http://struts.apache.org/download.cgi#struts258)
2. 创建Dynamic web project
3. 将jar包添加到WebContent\WEB-INF\lib目录下
4. build path到项目中
5.  在*web.xml*中添加过滤器
```
<filter>
	<filter-name>struts2</filter-name>
	<filter-class>
	org.apache.struts2.dispatcher.filter.StrutsPrepareAndExecuteFilter
	</filter-class>
</filter>
<filter-mapping>
	<filter-name>struts2</filter-name>
	<url-pattern>/*</url-pattern>
</filter-mapping>
```
6. 创建index.jsp  
添加：*<a href="helloworld.action">请求Struts2</a>*
7. 创建stuts.xml
```
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE struts PUBLIC
        "-//Apache Software Foundation//DTD Struts Configuration 2.5//EN"
        "http://struts.apache.org/dtds/struts-2.5.dtd">


<struts>
