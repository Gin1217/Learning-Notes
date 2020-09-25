# 9.24学习笔记

## 爬虫学习

- 入门程序
  - 网络爬虫是按照一定的规则，自动地抓取万维网信息的程序或者脚本。
  - 环境准备：JDK1.8，idea，idea自带的maven
  - 使用HttpClient技术抓取数据https://mvnrepository.com
- 网络爬虫介绍
- HttpClient抓取数据
- Jsoup解析数据
- 爬虫案例



### 示例

（在maven资源库网站中搜索HTTPClient和sfl4j）

1.在HttpClient中复制了maven框中的代码，粘贴进dependencies标签里

2.然后再复制sfl4j的maven框框中的代码粘贴

3.在resource文件夹下新建log4jfile然后敲入

、、、

```
log4j.rootLogger=Debug,A1;
log4j.logger.cn.itcast = DEBUG;

log4j.appender.A1=org.apache.log4j.ConsoleAppender;
log4j.appender.A1.layout=org.apache.log4j.PatternLayout;
log4j.appender.A1.layout.ConversionPattern=%-d{yyyy-MM-dd HH:mm:ss,SSS}
[%t] [%C]-[%p] %m%n
```

、、、

（算是配置好了）

4.爬取网页数据的几个步骤

- 打开浏览器，创建一个HttpClient对象
- 输入网址（HttpGet）
- 按回车，发起请求，返回响应，使用HttpClient对象发起请求
- 解析响应，获取数据，判断状态是否是200（HttpEntity）



### 遗留问题

<img src="/Users/gin/Library/Application Support/typora-user-images/截屏2020-09-2423.12.05.png" alt="截屏2020-09-2423.12.05" style="zoom:50%;" />



最后运行时显示错误：不支持发行版本 5**（淦）**

可能原因：Java版本不一致——项目编译配置使用的java版本不对

解决问题的参考方法：

链接在此：

<a href ="https://blog.csdn.net/Shiny0815/article/details/104794467?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522160095845619726892408758%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fall.%2522%257D&request_id=160095845619726892408758&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_v2~rank_v28-1-104794467.pc_first_rank_v2_rank_v28&utm_term=为什么会显示java%3A+错误%3A+不支持发行版本+5&spm=1018.2118.3001.4187">当idea里显示 "Java：错误：不支持发行版本时" 的解决方法</a>



- 第一步：file---Project Structure-- Project（将两版本改为一致）

- 第二步：file---Project Structure-- Modules（改为跟上面版本一样）

- 第三步：File---Preference for new  projects--build，execution，deployment--Java Compiler

  最后面那一条target 啥啥啥的地方改为一样的版本

  **然后我的问题就在这里！！我这里没有显示module！！点加号也没反应捏！！**

  **我 裂开 **

  **了**

  

![截屏2020-09-2423.18.12](/Users/gin/Library/Application Support/typora-user-images/截屏2020-09-2423.18.12.png)



1551我落泪了😭





调整了一下情绪，到现在已经是周五早上零点过了，我们宿舍还没熄灯，基本都在打代码，忽然有点温馨，有点感动。不知道为啥突然被治愈了啊哈哈哈。明天再新建一个库吧，不就是从头来过。



晚安。