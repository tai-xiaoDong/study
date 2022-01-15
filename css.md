# css 知识总结
## tai-xiaodong的博客 2022-1-15 饥人谷
### 一、浏览器渲染过程
1. 根据HTML构建HTML树  **（DOM）**
2. 根据css构建css树  **（CSSDOM）**
3. 将两棵树合并成一课渲染树 （render tree）
4. Layout 布局 （文档流，盒模型，计算大小和位置）
5. Paint 绘制（绘制边框颜色，文字颜色，影音等画出来）
6. Compose 合成（根据层叠关系展示画面）

~~~
个人理解
  1. html 主体内容 --> css 样式--> （平面）
  2. 计算 文档流,盒模型，大小位置等 -->(立体)
  3. 将这些合并渲染成网页
~~~

### 动画的做法

1.transitiong  自动补帧
~~~html
语法：transition 属性值 时长 过度方式 延迟
设置开始的样式和结束的样式，transition可以自动补充中间帧（transition要放在开始中）
语法 
1. 属性值 指定变化的方向等，例如 left right 等,可以使用all 指定所有
2. 时长  动画的长度  
3. 过渡方式 linear 线性匀速  ease 缓动  ease-in淡入 ease-out 淡出  ease-in-out  
4. 延迟 指定时间后开始  （常用单位 s  ms）
~~~
2.animation 关键帧
~~~html
需要设置keyframs
@keyframs 名字：{ 0%{状态}；100%{状态}；}； 或者 from{状态；to{状态}；}；
animation语法 （keyframs的）名字 延迟（同上）次数 
                           方向：reverse 反方向  alternate 交替  alternate-reverse结合使用
                           infinite alternate 无限循环
                           forwards 动画结束后 停在结束时的状态
                           paused 暂停 running 运行
~~~
3. (补充) transfrom 四种用法
~~~html
(注：元素必须是 block)
1.位移   语法: transform:translate 方向（距离);  
2.缩放   语法: transform:scale     方式 (倍数);
3.旋转   语法: transform:rotate    轴 (角度);
4.倾斜   语法: transform:skew      轴 (角度);
~~~


### 其他
    css的学习，需要多练习通过简单的操作组合从成美观的效果，除了普通的样式还有布局，动画等 
    
