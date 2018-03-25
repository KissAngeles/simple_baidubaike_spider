# simple_baidubaike_spider
新人小白为了学习python，按慕课网教程手打调试，也是为了给自己做个笔记总结

* python版本支持
  * 2.7

* 依赖库
  * BeautifulSoup，urllib2
  
* 项目概括
  * 可实现以百度百科python词条为入口抓取相关链接及简介并输出值html文件保存的功能
  * 程序包括爬虫调度端spider_main，URL管理器url_manager，网页下载器html_downloader，网页解析器html_parser以及数据输出模块html_outputer
  * 1、爬虫调度端spider_main，负责调用URL的管理，下载分析动作的执行，抓取结果的输出等各模块
  * 2、URL管理器url_manager，为url地址管理模块，包括add_new_url，add_new_urls，has_new_url，get_new_url这四个方法
  * 分别完成增加新URL到待爬取列表内，判断是否还有待爬取URL，获取待爬取URL并从待爬取列表内将其删除的操作
  * 3、网页下载器html_downloader，为网页下载模块，使用urllib2下载，并返回下载页面数据
  * 4、网页解析器html_parser，网页分析模块，调用BeautifulSoup，解析出下载到本地页面数据中的新URL及其简介并返回
  * 5、数据输出模块html_outputer，将抓取到的URL和简介数据保存在html格式文件内
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/%E6%95%B4%E4%BD%93%E7%BB%93%E6%9E%84.png)
  
* 思路图
  * 首先从入口URL（百度百科python页面）获取数据
  * 解析出其中的新URL和简介，新URL新增至URL管理器内new_urls列表，简介则连同对应URL新增至数据输出模块内datas列表
  * 此后根据新URL列表中URL重复“抓取”及“解析”的步骤，直至抓取数量计数器溢出停止，抓取的过程中如果出现页面失效等情况，可提示craw failed并跳过
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/%E6%80%9D%E8%B7%AF%E5%9B%BE.png)
  
* 项目开始
  * 执行spider_main.py即可

* 执行实例
  * 执行后可见抓取到了10个URL并打印，同时将URL及其简介保存在output.html文件内
  
  ![image](https://github.com/KissAngeles/simple_baidubaike_spider/blob/master/test.png)
