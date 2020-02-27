* **前言**
	
	本项目是基于C++线程池的轻量级Web并发服务器

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

	`cd ~/TinyWeb/Server/Codes`

	`./server 127.0.0.1 12345`
	
	(3).打开新终端，指定ip地址、端口、客户连接数运行压力测试程序：
	
	`cd ~/TinyWeb/Client/Codes`
	
	`./client 127.0.0.1 12345 1000`
