---
title:  "js基础知识罗列"
date:   2019-05-14 10:09:22 +0800
author: "廖艳丽"
---

### let 和 const 的区别

### 谈谈async和await这两个关键字

### es6新增的数组的方法

### rem的显示原理，移动端的rem设置方案

### hash模式和history模式

### npm和yarn的区别

### splice和slice的区别

### 节流函数和防抖函数

### for循环中的跳出

### 写出add(2)(5)的函数实现

### 以下代码的输出结果是什么？
```
function fun(n,o) {
    console.log(o);
    return{
        fun:function(m){
            return fun(m,n);
        }
    }
}
var a = fun(0);
a.fun(1);
a.fun(2);
a.fun(3);
var b = fun(0).fun(1).fun(2).fun(3);
```

### 说说Code Splitting

### js有哪些数据类型？

### !和!!的区别

### !==和!=的区别

### ===和==的区别

### vuetoast组件怎么解决多次调用问题？组件怎么挂载到全局？

### 手写webpack和一个vue组件

### 输出 0&&1,1&&1,1<2&&3>4,1<2&&0,-1&&3<4,0&&3<4,-0&&3<4的结果
0,1,false,0,true,0,-0

### 输出'1' + 2 + 3,1  + '2' + 3， 1 + 2 + '3',1 + 'a',1 + Number('a')的结果
```
"123","123","33","1a",NaN
```

### typeof,intanceof分别代表什么？

### vue计算属性的实现原理

### 如果让你手写一个类似vue的框架，你有什么思路？

### ts有没有用过？

### 箭头用CSS来书写

### 关键字有哪些？

### 全局变量和函数有哪些？

### 0/0,1/0,-1/0的结果是什么？
```
NaN,Infinity,-Infinity
```

### -0==0,-0===0的结果是什么？



