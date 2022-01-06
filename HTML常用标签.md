# HTML 常用标签
## Tai-xiaoDong  2022.1.6 来源 饥人谷


### 一. a 标签的用法

1. 网页跳转
~~~html
<a href="网址">指定页面</a> 
~~~
2. 内部锚点跳转
~~~html
<a href="#xxx">指定锚点</a> (跳转到id为xxx的标签)
~~~
3. 伪协议
~~~html
<a href="javascritp : ;"> 自定义名称</a>   <!-- 创建一个什么也不做的空标签 -->
<a href="mailto:邮箱地址"> 自定义名称</a>   <!-- 创建可以给指定邮箱发邮件的标签 -->
<a href="tel：手机号"> 自定义名称</a>       <!-- 创建一个呼叫指定电话的标签 -->
~~~
4. 其他属性
~~~html
<a target="_blank">  <!-- 在新页面打开 ,默认是 "_self"-->
<a target="_top">    <!-- 在最顶层页面打开-->
<a target="_parent"> <!-- 在当前页面上一级打开-->
<a target="自定义名称"> <!-- 在自定义名称的页面中打开，如果没有该页面就新建一个-->
~~~

### 二. img 标签的用法
~~~html
<img src="图片路径或地址">  <!--发出一个get请求访问该图片-->
<img width=宽  height=高 alt=图片加载失败时候显示指定内容> <!--宽和高只设定一个，另一个会自适应调整，永远不要让图片变形-->
~~~

### 三. table 标签的用法
~~~html
<thead> <!--顶部-->
  <tr>  <!--行-->
    <th></th> <!--表头-->
  </tr>
</thead>
<tbody>
  <tr>
    <td></td>
  </tr>
</tbody>
<tfoot>  <!--底部-->
  <tr>
    <td></td> <!--普通单元格-->
  </tr>
</tfoot>

日常表结构如下：
thead tr th th th th th tr thead
tbody tr th td td td td tr 
      tr th td td td td tr tbody
tfoot tr th td td td td tr tfoot 
~~~

### 四. 其他感想
~~~
可以明显感觉到，从这里开始，知识量逐步在增加，难度也在提高，实际上非常好理解，但是一定要多动手实操，试验。
~~~
