# HTML 入门笔记1

### Tai-xiaoDong个人学习笔记，来源饥人谷前端学员


## 一  起源
~~~
HTML是由web的发明者 Tim Berners-Lee 李爵士发明
~~~



## 二  HTML起手式
~~~
1. <!DOCTYPE html>      <!-- 告诉浏览器文档类型 -->

2. <html lang="zh-CN">    <!-- 根标签，lang属性即 language en 为英文  zh为中文  -->

3. <head>      <!-- 一般是用户不可见的内容 -->   

4. <meta charset="UTF-8">     <!-- 文件的字符编码 -->    

5. <meta http-equiv="X-UA-Compatible" content="IE=edge">    <!-- 无需更改，告诉IE浏览器使用最新内核 -->   

6. <meta name="viewport" content="width=device-width, initial-scale=1.0">    <!--  禁用缩放兼容手机  -->  

7. <title>导航栏的标题</title>

8. </head>

9. <body>  <!--网页显示的主要内容-->

10. </body>

11. </html>
~~~


## 三 HTML 常见的章节标签
~~~
1. <h1> ~ <h6>      标题标签  一般一个网页只有一个h1   1最大 6最小

2. <section>        章节标签  其中间的代码是一个新的章节，可以重新使用h1-h6

3. <main>           主体部分

4. <header>         最顶部位置的内容

5. <footer>         最底部位置的内容，多用来写版权声明   &copy 是 ©版权符号

6. <div>            将内容分块

7. <aside>          旁支内容，main以外的内容 用于导航栏等
~~~


## 四  HTML 的全局属性
~~~
1. class       类  可以使标签有相同的类别，css可以根据class 统一添加样式

2. title       鼠标移动到该标签处 显示指定的内容

3. hidden      隐藏一个标签，可以使用css恢复

4. id          给标签起名字，应具有唯一性，但是不唯一也不报错，尽量不要使用，css和js都可以通过id 调用标签。

5. style       通过html语句设置标签样式，优先级高于css  低于js

6. tabindex    指定用户使用tab键时的选中顺序，从 1开始，o是最后一个  -1表示不会被选中

7.contenteditable    使一个标签可以被用户更改

~~~



## 五  常见的内容标签
~~~
 1. <ol><li>    顺序显示  类似于excel的项目编号
 
 2.  <ul><li>   无序显示  类似于excel的项目符号 显示黑色圆点
 
 3. <dl>        描述性语句  <dt>描述物标题或名字   <dd>描述语句
 
 4. <pre>       浏览器默认不保留多个空格等，pre标签中的会得到保留
 
 5. <hr>        分隔线
 
 6. <br>        换行
 
 7. <a>         插入链接
 
 8. <em>        斜体 表示语气的重视 
 
 9. <strong>    加粗  表示本身的重要
 
 10. <p>        段落  块级  会在段前段后增加缩进
 
 11. <code>     使字符等宽
 
 12. <quote>    表示引用 但是没有什么特殊的显示效果
 
 13. <blackquote>  作用和p类似，但是应用于句子中
~~~


* 注：标签可以嵌套使用来达到特殊的效果


