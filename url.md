# 浅析URL
## Tai-xiaoDong 2022.1.16 饥人谷

### 一、URL包括哪几部分，每部分的作用是什么

~~~
Uniform Resource Locator
一个完整的 URL 由：协议 域名 路径 查询参数 锚点 组成
协议 负责和服务器通信
域名 表示服务器的地址
路径 表示查询的页面
查询参数 表示在相同页面要查找的值
锚点 定位到指定页面的指定位置
~~~
### 二、DNS的作用是什么，nslook命令怎么用？
~~~
DNS 负责使域名和IP对应起来
“浏览器” > 向服务器发起请求 > “服务器” > 返回Ip地址 > “浏览器” > 访问对应IP
nslook  可以向服务器查询对应域名的IP地址
~~~
### 三、IP的作用是什么，ping命令怎么用？
~~~
IP的作用 ：1.定位一台设备  2.封装数据报文，以跟其他设备交流
ping： ping 域名  会返回对应的IP地址
~~~
### 四、域名是什么 分为哪几类域名？
~~~
Internet上某一台计算机或计算机组的名称，用于在数据传输时对计算机的定位标识（有时也指地理位置）（百度百科）
分为  1.com等顶级域名
      2.xxx.com 二级域名（俗称一级）
      3.www.xxx.com 三级域名（俗称二级）
2和3是父子关系，可以不是同一家公司 也可以是，www是多余的。
~~~
