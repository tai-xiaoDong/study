#  JQuery 简述
#### tai-xiaodong 2022年2月1日 饥人谷

### Demo
在开始之前我想先记录一点自己的想法。
1. 这些想法是我刚刚上完课的个人理解并未看过任何相关文档，因此一定会有错误和疏漏
* jQuery是一个操作Dom 的库，相比于原生js 以及第一次封装的Dom库，它更加的简洁易用，核心在于‘this’
* 我喜欢把jQuery看做是一个构造函数，它通过参数调用筛选出需要操作的标签，并以此构建一个对象api，通过函数闭包的形式实现功能
* 由于筛选出的标签可能有多个，所以对象中的函数大部分都需要通过for循环来遍历操作或者二次筛选
* 这些函数如果层级未发生改变，则返回this（即这个对象本身）这样可以继续调用他的函数实现链式操作
* 如果函数层级发生改变，当前操作的对象变成父级子级等，需要将当前对象返回给jQuery，重新赋值给对象，此时this发生改变，同样继续实现链式操作
* 一些共有的api可以写入到jQuery.prototype中节省内存

## 下面写一下JQuery的一些常用功能
1. jQuery 如何获取元素
2. jQuery 的链式操作是怎样的
3. jQuery 如何创建元素
4. jQuery 如何移动元素
5. jQuery 如何修改元素的属性
注 jQuery的别名为$

~~~js
1. jQuery 如何获取元素

    $(document) //选择整个文档对象

　　$('#test') //选择ID为test的网页元素

　　$('div.className') // 选择class为className的div元素

　　$('input[name=first]') // 选择name属性等于first的input元素
  
    这些获取到的元素会传递给对象，通过对象的api对他们进行操作
~~~
~~~js
2. jQuery 的链式操作是怎样的

　 $('#test').find('child').className('Hello');
  
   这样的操作主要是依靠函数返回的是this 而不是值。这样就可以继续调用this内的函数
~~~
~~~js
3. jQuery 如何创建元素

   jQuery创建元素的方式非常简单只需要传递不同的参数。其内部的同有属性就可以直接使用
   
   let api=jQuery（'#test'）
~~~
~~~js
4. jQuery 如何移动元素

    .insertAfter()和.after()：在现存元素的外部，从后面插入元素

　　.insertBefore()和.before()：在现存元素的外部，从前面插入元素

　　.appendTo()和.append()：在现存元素的内部，从后面插入元素

　　.prependTo()和.prepend()：在现存元素的内部，从前面插入元素
~~~
~~~js
5. jQuery 如何修改元素的属性

   通过addClass（className）添加对应属性
~~~
### 后记
jQuery是一个快速、简洁的JavaScript库，于2006年发布。jQuery写更少的代码，做更多的事情。
它封装JavaScript常用的功能代码，提供一种简便的JavaScript设计模式，优化HTML文档操作等

* 闭    包：  函数调用外部变量，这个函数和这个变量就形成了闭包
* 适 配 器：  代码对不同运行环境都做了适配
* 链式操作：  链式调用的核心，就是函数在执行完成后，返回了this，即当前对象
* 重    载： 一个函数支持的参数有多种不同的状态
