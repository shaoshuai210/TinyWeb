* **前言**
	
	本项目是基于C++线程池的轻量级Web并发服务器,事件处理模式采用Reactor模式，主线程只负责监听文件描述符是否有事件发生，读写数据、接收新的连接、以及处理客户请求均在工作线程中实现；使用半同步/半异步模式，每个线程（主线程和工作线程）都通过一个epoll维护自己的事件循环，它们各自独立地监听不同事件。

* **运行环境**

	(1).系统：Ubuntu16.04;
	
	(2).语言：C++ 11及以上版本;

* **支持功能**
	
	(1).支持Get请求;
	(2).支持长连接/短连接;
	(3).支持ipv4;(4).支持tcp;(5).支持请求静态内容(6).支持并发请求
	
* **开始运行**

	(1).下载程序;

	`git clone git@github.com:Buerzhu/TinyWeb.git`
	
	(2).打开新终端，指定ip地址和端口运行服务器程序：

	`cd ~/TinyWeb/Server/Debug`

	`./server 127.0.0.1 12345`
	
	(3).打开新终端，指定ip地址、端口、客户连接数运行压力测试程序：
	
	`cd ~/TinyWeb/Client/Debug`
	
	`./client 127.0.0.1 12345 1000`
