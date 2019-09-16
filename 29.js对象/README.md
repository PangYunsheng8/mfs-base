### 问答题
##### 1. 创建对象有几种方式？最常用的是那种？
有三种创建对象的方式，分别是直接创建、使用字面量创建和对象构造器创建。最常用的是字面量创建。
##### 2. 如何使用对象构造器？对象构造器和函数有什么关系？
用对象构造器来创建对象的方法如下：
function Person(name,age){
    this.name=name;
    this.age=age;
}
var myName=new Person("pys",21);
它是通过函数的方法来创建对象，函数体内规定了对象的所有属性。
##### 3. 如何遍历所有的对象属性？
可以使用for...in循环遍历所有的对象属性，如：
var person={fname:"Bill",lname:"Gates",age:56};
for (x in person){
  console.log(x, person[x])
}

---
### 代码题
https://github.com/PangYunsheng8/mfs-homework/blob/master/29.js%E5%AF%B9%E8%B1%A1/homework29.html
