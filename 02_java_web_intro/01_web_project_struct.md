# JavaWeb项目结构

项目结构, 也就是项目中各个组成部分的目录结构。

大体上可以分为2种类别, 一种是开发过程中的目录结构, 另一种是打包完成后的war包目录结构。

首先我们来看常规的 war 包目录结构。

```
--MyWebApp (dir)
  |--WEB-INF (dir)
     |--web.xml (必须)
     |--classes (目录)
     |--lib (目录)
  |--index.jsp (可选)
```


> war包, Web压缩文件(web archive)的缩写。 其本质是JAR文件格式, 只是把后缀给改成 `.war`, 以便于区分。其中一般包含: servlet相关的class文件, web文件,支持文件,图片,以及HTML等等,当然,还可以包含web应用说明信息。

[Spring.io页面](https://spring.io/understanding/WAR) 有如下说明:


Understanding WAR
WAR (Web application ARchive) files are used to distribute Java-based web applications. A WAR has the same file structure as a JAR file, which is a single compressed file that contains multiple files bundled inside it.

WAR files are used to combine JSPs, servlets, Java class files, XML files, javascript libraries, JAR libraries, static web pages, and any other resources needed to run the application.

WAR files are usually deployed in servlet containers, but can also be deployed to Java EE application servers. When a WAR file is deployed to a container, the container usually unpacks it to access the files and then launches the application. With servlet containers being the most prolific platform for Java web applications, WAR files are not only a Java spec standard, but a very common format for distributing Java applications and supported by a wide range of tools.

WAR files cannot be edited while the application is running. Any changes require rebuilding the file.


JavaEE7规范: <https://docs.oracle.com/javaee/7/tutorial/packaging003.htm>



