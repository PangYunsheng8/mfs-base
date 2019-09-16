### 问答题
##### 1. 为什么会有函数？函数有什么用？
函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块，使用函数可以使得代码更加简便，避免写过多的重复语句。
##### 2. 有哪几种声明函数的方式？最常用的是哪些？
1）可以使用Function()构造函数来声明：
var myFunction = new Function("a", "b", "return a+b");
2）使用function关键字声明：
function myFunction(a, b){
    return a+b;
}
3）使用函数表达式来声明：
var myFunction = function(a, b){return a+b};
##### 3. 声明是函数返回值？如何设置函数返回值？如何获得函数返回值？
返回值是函数执行后的反馈，可以通过return来设置函数的返回值，可以声明一个变量，将函数的返回值赋给这个变量获取这个
返回值。
##### 4. 函数中 return 后面的语句会执行吗？为什么？
不会，因为到return时，函数已经结束。
##### 5. 声明是函数提升？为什么会有函数提升？
函数提升是 JavaScript 默认将当前作用域提升到前面去的的行为，函数声明使得函数可以在声明之前调用。

---
### 代码题
https://github.com/PangYunsheng8/mfs-homework/blob/master/28.js%E5%87%BD%E6%95%B0/homework28.html