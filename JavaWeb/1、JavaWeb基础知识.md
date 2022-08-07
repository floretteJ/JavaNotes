# 一、基本概念

## 1、前言

web开发：

- web，网页的意思，www.baidu.com·


- 静态web
  - html,sss
  - 提供给所有人看的数据始终不会发生变化！

- 动态web

  - 淘宝，几乎是所有的网站；

  - 提供给所有人看的数据始终会发生变化，每个人在不同的时间，不同的地点看到的信息各不相同！

  - 技术栈：Servlet/ISP，ASP，PHP

    

## 2、web应用程序

- 可以提供浏览器访问的程序；
- a.html、b.html.….多个web资源，这些web资源可以被外界访问，对外界提供服务；
- 你们能访问到的任何一个页面或者资源，都存在于这个世界的某一个角落的计算机上。
- URL
- 这个统一的web资源会被放在同一个文件夹下，web应用程序>Tomcat：服务器
- 一个web应用由多部分组成（静态web，动态web)
  - html,sss,is
  - jsp,servlet
  - Java程序
  - jar包
  - 配置文件（Properties)

Web应用程序编写完毕后，若想提供给外界访问；需要一个服务器来统一管理。



## 3、静态web

- *.htm, *.html,这些都是网页的后缀，如果服务器上一直存在这些东西，我们就可以直接进行读取。

![img](https://img-blog.csdnimg.cn/20200517145610480.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NjM5MDQzMw==,size_16,color_FFFFFF,t_70)

- 静态web存在的缺点

  - Web页面无法动态更新，所有用户看到都是同一个页面

    - 轮播图，点击特效：伪动态

    - JavaScript [实际开发中，它用的最多]
    - VBScript

  - 它无法和数据库交互（数据无法持久化，用户无法交互）



## 4、动态web

- 页面会动态展示： “Web的页面展示的效果因人而异”；

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200517145638566.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NjM5MDQzMw==,size_16,color_FFFFFF,t_70)

- 缺点：
  - 加入服务器的动态web资源出现了错误，我们需要重新编写我们的后台程序,重新发布；
  - 停机维护；

- 优点：
  - Web页面可以动态更新，所有用户看到都不是同一个页面
  - 它可以与数据库交互 （数据持久化：注册，商品信息，用户信息…）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200517145733386.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NjM5MDQzMw==,size_16,color_FFFFFF,t_70)



# 二、web服务器

## 1、技术讲解

**ASP:**

- 微软：国内最早流行的就是ASP；
- 在HTML中嵌入了VB的脚本， ASP + COM；
- 在ASP开发中，基本一个页面都有几千行的业务代码，页面极其换乱
- 维护成本高！
- C#
- IIS

**php：**

- PHP开发速度很快，功能很强大，跨平台，代码很简单 （70% , WP）

无法承载大访问量的情况（局限性）

**JSP/Servlet : **

B/S：浏览和服务器

C/S: 客户端和服务器

- sun公司主推的B/S架构
- 基于Java语言的 (所有的大公司，或者一些开源的组件，都是用Java写的)
- 可以承载三高问题带来的影响；
- 语法像ASP ， ASP–>JSP , 加强市场强度；



## 2、web服务器

服务器是一种被动的操作，用来处理用户的一些请求和给用户一些响应信息；

**IIS**

- 微软的； ASP…,Windows中自带的

**Tomcat**

- Tomcat 服务器是一个免费的开放源代码的Web 应用服务器，属于轻量级应用[服务器](https://baike.baidu.com/item/服务器)，在中小型系统和并发访问用户不是很多的场合下被普遍使用，是开发和调试JSP 程序的首选。
- 对于一个Java初学web的人来说，它是最佳的选择。



## 3、Tomcat

### 3.1 安装Tomcat

tomcat官网：http://tomcat.apache.org/



### 3.2 Tomcat的启动和配置

![img](https://img-blog.csdnimg.cn/20200517150516571.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NjM5MDQzMw==,size_16,color_FFFFFF,t_70)

访问测试：http://localhost:8080/

可能遇到的问题：

1. Java环境变量没有配置
2. 闪退问题：需要配置兼容性
3. 乱码问题：配置文件中设置



### 3.3 配置

- Tomcat安装目录下的conf下的server.xml文件

- 可以配置启动的端口号
  - tomcat的默认端口号为：8080
  - mysql：3306
  - http：80
  - https：443

```java
<Connector port="8081" protocol="HTTP/1.1"
           connectionTimeout="20000"
           redirectPort="8443" />
```

- 可以配置主机的名称
  - 默认的主机名为：localhost->127.0.0.1
  - 默认网站应用存放的位置为：webapps

```java
 <Host name="www.florette.com"  appBase="webapps"
        unpackWARs="true" autoDeploy="true">
```

**高难度面试题：**
请你谈谈网站是如何进行访问的！

1、输入一个域名；回车

2、检查本机的 C:\Windows\System32\drivers\etc\hosts配置文件下有没有这个域名映射；

- 有：直接返回对应的ip地址，这个地址中，有我们需要访问的web程序，可以直接访问


```java
127.0.0.1       www.florette.com
```



- 没有：去DNS服务器找，找到的话就返回，找不到就返回找不到
  - 去请求DNS服务器，通过DNS获取相应的域名对应的IP
  - 然后通过IP地址找到IP对应的服务器后，要求建立TCP连接
  - 浏览器发送完HTTP Request（请求）包后，服务器接收到请求包之后才开始处理请求包
  - 在服务器收到请求之后，服务器调用自身服务，返回HTTP Response（响应）包
  - 客户端收到来自服务器的响应后开始渲染这个Response包里的主体（body），等收到全部的内容随后断开与该服务器之间的TCP连接。



### 3.4 发布一个web网站

- 将自己写的网站，放到服务器(Tomcat)中指定的web应用的文件夹（webapps）下，就可以访问了。
- 网站应该有的结构

```java
--webapps ：Tomcat服务器的web目录
	-ROOT
	-florettestudy ：网站的目录名
		- WEB-INF
			-classes : java程序
			-lib：web应用所依赖的jar包
			-web.xml ：网站配置文件
		- index.html 默认的首页
		- static 
            -css
            	-style.css
            -js
            -img
         -.....

```

- HTTP协议 ： 面试

- Maven：构建工具
  - Maven安装包

- Servlet 入门
  - HelloWorld！
  - Servlet配置
  - 原理



## 4、Http

### 4.1 什么是HTTP

HTTP（超文本传输协议）是一个简单的请求-响应协议，它通常运行在TCP之上。

- 文本：html，字符串，~ ….
- 超文本：图片，音乐，视频，定位，地图…….
- 80

Https：安全的

- 443



### 4.2 两个时代

- http1.0
  - HTTP/1.0：客户端可以与web服务器连接后，只能获得一个web资源，断开连接
- http2.0
  - HTTP/1.1：客户端可以与web服务器连接后，可以获得多个web资源。



### 4.3 Http请求

- 客户端—发请求（Request）—服务器

- 请求行
  - 请求方法：Get，Post，HEAD,DELETE,PUT,TRACT…
    - get：请求能够携带的参数比较少，大小有限制，会在浏览器的URL地址栏显示数据内容，不安全，但高效
    - post：请求能够携带的参数没有限制，大小没有限制，不会在浏览器的URL地址栏显示数据内容，安全，但不高效。
  - URL
  - 协议版本：HTTP/主版本号.次版本号
    - HTTP/1.0
    - HTTP/1.1

- 请求头

```java
Accept：告诉浏览器，它所支持的数据类型
Accept-Encoding：支持哪种编码格式  GBK   UTF-8   GB2312  ISO8859-1
Accept-Language：告诉浏览器，它的语言环境
Cache-Control：缓存控制
Connection：告诉浏览器，请求完成是断开还是保持连接
HOST：主机..../.
```

注意点：请求头部的最后会有一个空行，表示请求头部结束，接下来为请求正文，这一行非常重要，必不可少。

- 请求正文（可选）



### 4.4 Http响应

- 服务器—响应（Response）-----客户端

- 状态行
  - 状态码
  - 状态码描述
  - 协议版本

```java
200： 响应成功
301： 永久重定向，搜索引擎将删除源地址，保留重定向地址
302： 暂时重定向，重定向地址由响应头中的Location属性指定（JSP中Forward和Redirect之间的区别）
      由于搜索引擎的判定问题，较为复杂的URL容易被其它网站使用更为精简的URL及302重定向劫持
304： 缓存文件并未过期，还可继续使用，无需再次从服务端获取
400： 客户端请求有语法错误，不能被服务器识别
403： 服务器接收到请求，但是拒绝提供服务（认证失败）
404： 请求资源不存在
500： 服务器内部错误 
```

- 响应头

```java
Accept：告诉浏览器，它所支持的数据类型
Accept-Encoding：支持哪种编码格式  GBK   UTF-8   GB2312  ISO8859-1
Accept-Language：告诉浏览器，它的语言环境
Cache-Control：缓存控制
Connection：告诉浏览器，请求完成是断开还是保持连接
HOST：主机..../.
Refresh：告诉客户端，多久刷新一次
Location：让网页重新定位
```

- 响应正文

**常见面试题：**

当你的浏览器中地址栏输入地址并回车的一瞬间到页面能够展示回来，经历了什么？



## 5、Maven

**为什么要学习这个技术？**

1. 在Javaweb开发中，需要使用大量的jar包，我们手动去导入；

2. 如何能够让一个东西自动帮我导入和配置这个jar包。

   由此，Maven诞生了！

### 5.1 Maven项目架构管理工具

我们目前用来就是方便导入jar包的！

Maven的核心思想：**约定大于配置**

- 有约束，不要去违反。

Maven会规定好你该如何去编写我们的Java代码，必须要按照这个规范来；



### 5.2 下载安装Maven

官网：https://maven.apache.org/

下载完成后，解压即可；



### 5.3 配置环境变量

在我们的系统环境变量中

配置如下配置：

- M2_HOME： maven目录下的bin目录
- MAVEN_HOME： maven的目录
- 在系统的path中配置 %MAVEN_HOME%\bin

![image-20210622142758069](../AppData/Roaming/Typora/typora-user-images/image-20210622142758069.png)

测试Maven是否安装成功，保证必须配置完毕！



### 5.4 阿里云镜像

打开maven安装目录下的conf/settings.xml文件

在<mirrors></mirrors>中添加如下配置：

```java
<mirror>
      <id>nexus-aliyun</id>
	  <mirrorOf>central</mirrorOf>
	  <name>Nexus aliyun</name>
  <url>http://maven.aliyun.com/nexus/content/repositories/central/</url>
</mirror>
```



### 5.5 本地仓库

maven有本地仓库和远程仓库；
**建立一个本地仓库**（同样在settings.xml中）

```java
<localRepository>E:\maven\apache-maven-3.6.3\maven-repo</localRepository>
```



### 5.6 在IDEA中使用Maven(看文件)

### 5.7 创建一个普通的Maven项目

### 5.8 标记文件夹功能

### 5.9 在 IDEA中配置Tomcat

### 5.10 pom文件（Maven核心配置文件）

maven由于他的约定大于配置，我们之后可以能遇到我们写的配置文件，无法被导出或者生效的问题，解决方案如下：

```java
<!--在build中配置resources，来防止我们资源导出失败的问题-->
<build>
    <resources>
        <resource>
            <directory>src/main/resources</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>false</filtering>
        </resource>
        <resource>
            <directory>src/main/java</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>false</filtering>
        </resource>
    </resources>
</build>
```



### 5.11 IDEA操作

### 5.12 解决遇到的问题

1. Maven 3.6.2

   解决方法：降级为3.6.1

   ![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-eHFd6K4o-1589699013817)(JavaWeb.assets/1567904721301.png)]](https://img-blog.csdnimg.cn/20200517152055888.png)

2. Tomcat闪退

3. IDEA中每次都要重复配置Maven
   在IDEA中的全局默认配置中去配置

4. Maven项目中Tomcat无法配置
5. maven默认web项目中的web.xml版本问题

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-B3V2w3Es-1589699013818)(JavaWeb.assets/1567905537026.png)]](https://img-blog.csdnimg.cn/20200517152201837.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NjM5MDQzMw==,size_16,color_FFFFFF,t_70)

6. 替换为webapp4.0版本和tomcat一致

   ```java
   <?xml version="1.0" encoding="UTF-8"?>
   <web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee
                         http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
            version="4.0"
            metadata-complete="true">
   
   </web-app>
   ```

7. Maven仓库的使用

- 地址：https://mvnrepository.com/



































