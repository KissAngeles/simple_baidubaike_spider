# simple_baidubaike_spider
新人小白为了学习python，按慕课网教程手打调试，也是为了给自己做个笔记总结

* python版本支持
  * 2.7

* 依赖库
  * BeautifulSoup，urllib2
  
* 项目概括
  * 可实现以百度百科python词条为入口抓取相关链接及简介并输出值html文件保存的功能
  * 程序包括爬虫调度端spider_main，URL管理器url_manager，网页下载器html_downloader，网页解析器html_parser以及数据输出模块html_outputer
  * 1、爬虫调度端spider_main，负责调度，包括URL的管理，下载分析动作的执行，抓取的结果的输出
  * 2、
  * 3、
  * 4、
  * 5、
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/%E6%95%B4%E4%BD%93%E7%BB%93%E6%9E%84.png)
  
* 思路图
  * XX
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/%E6%80%9D%E8%B7%AF%E5%9B%BE.png)
  
* 项目开始
  * 执行spider_main.py即可

* 对应文件说明
  * html_downloader.py  网页下载模块，使用urllib2下载
  * html_outputer.py  抓取到的数据保存在html文件内
  * html_parser.py  网页分析模块，调用BeautifulSoup
  * output.html 保存抓取到的网页数据
  * spider_main.py  主运行目录
  * url_manager.py  url地址管理模块

* 执行实例
  * XX
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/test.png)
