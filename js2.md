# Javascript 对象的基本用法

### Tai-xiaodong 饥人谷 2022.1.23

#### 1.声明对象的两种用法
~~~js
1. let obj={key值:value值,key值:value值}
2. let obj=new object{key:value}

key值 的单引号在某些时候可以省略，但是key值永远是一个字符串
~~~

#### 2.如何删除对象属性
~~~js
1. delete 对象名.属性名   //直接删除属性和属性值
2. 对象名.属性名=undefined   //删除对象的属性值
~~~
#### 3.如何查看对象属性
~~~js
Object.keys(对象名）  //查看对象所有的属性名
Object.values(对象名) //查看对象所有属性值
console.dir(对象名)   //查看对象的所有属性，包括共有属性
对象名.__proto__      //直接查询共有属性
~~~
#### 4.如何增加和修改对象的属性
~~~js
1. 通过赋值的方式  如果原本有属性值是修改，如果没有就是增加
2. Object.assign(对象名，{key:value,key:value}) //多个值赋值 同上 这些修改和增加都不影响共有属性
3. 修改共有属性的方法：
    （1）Object.prototype.tostring='xxx'
    （2）obj.__proto__.tostring='xxx'  
    //推荐使用第二种，一般不要修改共有属性，会引起很多问题。
~~~

#### 5 两种判断属性的方法
~~~js
1. 属性名 in 对象名  //如果是true 那么这个对象就拥有该属性
2. obj.hasOwnProperty('属性名') // 判断该属性是这个对象的共有属性还是私有属性
~~~
