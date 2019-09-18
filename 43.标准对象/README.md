### 问答题
##### 1. JavaScript 有哪些常用的标准对象？
Javascript有三个常用的标准对象：Math, Date, JSON。
##### 2. Math 对象有哪些常用方法和常量？
Math中的常用常量有：
1)Math.E: 算数常量e(约等于2.718)
2)Math.PI: 圆周率(约等于3.1415)
3)Math.SQRT2: 2的平方根(约等于1.414)
Math中的常用方法有：
1)abs(x):返回绝对值
2)ceil(x):向上取整
3)floor(x):向下取整
4)round(x):四舍五入
5)random():
6)max(x,y):取最大值
7)min(x,y):取最小值
8)log(x):log函数
9)exp(x):e 的指数
10)sin(x)/cos(x)/tan(x):正弦/余弦/正切
##### 3. 如何获取当前时间？如何根据需要构建 Date 对象？
获取当前时间可以通过初始化一个Date对象：
```
var myDate=  new Date();
```
##### 4. 什么是 JSON？JSON 在 JavaScript 中是什么数据类型？在网页构建的过程中，我们常用 JSON 来干什么？
JSON是一种轻量级数据交换格式，JSON在JavaScript中的数据类型是字符串，在网页构建中，JSON 对象主要用来序列化和反序列化 JavaScript 对象。
##### 5. 如何将 JSON 转化为 JavaScript 中的 Object？
使用JSON.parse()方法。
##### 6. 如何将 JavaScript 中的 Object 转化为 JSON ？
使用JSON.stringify()方法。

---
### 代码题