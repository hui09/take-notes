### http协议

http://www.ydma.cn/courses/RbG4Be1Wn

服务器状态：客户端向服务器发送消息响应码

```
2：成功；
3：你要的东西以前有现在没有
404：服务器没有数据，
403：没有权限
5：服务器问题
```

pipe:管道

协议头:hand  描述信息

协议体：body  写的内容；

'text/  plain  文本块

res.write 发送后不断开链接

res.end 发送后并断开链接

动态网站 ：数据是由后端服务器语言生成的，改变后端数据前端就会发生变化，方便维护

强交互：实时的

http    ：协议是最廉价 最容易搭建起来的协议，支持大量开元项目，节约资源 

GET    ：客户端向服务器发送请求数据是在头文件里面解析数据的

POST ：客户端向服务器发送请求先是头文件响应数据还未接收到

### 1.HTTP：是一种超文本传输协议，用于WWW服务器传输文本到本地浏览器的传输协议，

```
        1.客户端请求页面数据，http协议名  主机名  端口号    路径
		2.封装http请求包数据
		3.分装成TCP包，建立TCP的三次握手四次挥手
		
		 4.在HTTP工作开始之前，客户机（Web浏览器）首先要通过网络与服务器建立连接，该连接是通过TCP来完成的，该                   协议与IP协议共同构建Internet，即著名的TCP/IP协议族，因此Internet又被称作是TCP/IP网络。HTTP是比TCP更                   高层次的应用层协议，根据规则，只有低层协议建立之后才能进行更高层协议的连接，因此，首先要建立TCP连                       接，一般TCP连接的端口号是80。
	    4.客户机发送请求命令
		       建立链接后客户机发送请求服务器请求方式通过URL、协议版本号  客户机信息和可能的内容，
		5.服务器响应
		        服务器请求后  给予响应信息成功或错误代码   
		 6.服务器关闭TCP链接
		         一般情况下，一旦Web服务器向浏览器发送了请求数据，它就要关闭TCP连接，然后如果浏览器或者服务器在其头信息加入了这行代码
			
```

### 2.TCP/IP ：TCP是一种传输控制协议。

```
1..TCP是应用层协议：
            提供了无差错的数据传输，按序传输（数据总是会按照发送的顺序到达）
            末分段的数据流(可以任意时刻以任意尺寸将数据发送出去)   
```

### 3.UDP和TCP有什么区别

     1、TCP面向连接（如打电话要先拨号建立连接）;UDP是无连接的，即发送数据之前不需要建立连接
    
    2、TCP提供可靠的服务。也就是说，通过TCP连接传送的数据，无差错，不丢失，不重复，且按序到达;UDP尽             最大努力交付，即不保证可靠交付 ，Tcp通过校验和，重传控制，序号标识，滑动窗口、确认应答实现可靠           传输。如丢包时的重发控制，还  可以对次序乱掉的分包进行顺序控制。
    
     3.UDP具有较好的实时性，工作效率比TCP高，适用于对高速传输和实时性有较高的通信或广播通信。
     4.每一条TCP连接只能是点到点的;UDP支持一对一，一对多，多对一和多对多的交互通信。
    
     5、TCP对系统资源要求较多，UDP对系统资源要求较少。

### 4.URL：

```
URL：全球资源统一定位符   是一个完整的网络地址  http协议 +主机地址  +服务器端路径 +获取字符串rg

1.浏览器从URL中解析出服务的主机名
2.浏览器将服务器的主机名转化服务器的IP地址；
3.浏览器将端口号（如果没有的话）从URL中解析出来；
4.浏览器建立一条与WEB服务器的TCP 链接
5.浏览器向服务器发送一条HTTP请求报文
6.服务器向浏览器回送一条HTTP响应报文
7.关闭链接，浏览器显示文档。
```

### 5.socket

   ```
socket：接口      套接字
socket：是一种双向实时网络链接
   ```

#### 6.连接：

```
短连接：
        指服务端与客户端每次完成通讯后，就断开链接套接字的链接，同时每次需要服务端与客户端产生通		讯的时候，都要重新创建套接字，HTTP默认使用长连接。
长连接：
        只需要一个套接字就能完成与服务器端所有的通讯，客户端只需开始要创建一个套接字便可以和服务           器 多次反复通讯
```







































