### 代码题
1. 请写出能匹配如下数的正则表达式
1)整数：
2)非负浮点数
3)正浮点数
4)非正浮点数
5)负浮点数
6)浮点数


(^-?[1-9]\d*$)|0


2. 请写出可以检查用户名的正则表达式，要求如下
1)其长度为8-16个字符
2)以字母开头
3)可以包含数字、下划线
/^[a-zA-Z][0-9_]{7,15}/
3. 请写出可以匹配所有合法电子邮箱的正则表达式
^[\w]+(\.[\w]+)*@[\w]+\.com$
4. 请写出可以检查是否是合法网址的url(可以是http协议或者https协议)
/^https?:\/\/$/
5. 请完成checkPassword(str)这个函数，这个函数可以检查用户输入的密码是否合法，以下是密码要求
1)6-16个字符
2)首字符为字母或者下划线
3)应该包括小写字母，大写字母，数字，下划线中的至少3个
4)不能包括其他特殊字符
function checkPassword(str){
    var reg = /^(?![a-zA-Z]+$)(?![a-z\d]+$)(?![a-z_]+$)(?![A-Z\d]+$)(?![A-Z_]+$)(?![\d_]+$)[a-zA-Z_][a-zA-Z0-9_]{5,15}$/
    if reg.test(str){
        return true;
    }
    else{
        return false;
    }
}
6. 请使用正则表达式实现jQuery中的addClass和removeClass
```
def addClass(str,clazz){
   var reg = new RegExp("\b" + clazz + "\b");
   if (reg.test(str)){
       return str;
   }
   else{
       return str + " " + clazz;
   }
}
def removeClass(str,clazz){
    var reg = new RegExp("\b" + clazz + "\b");
       if (reg.test(str)){
           return str.replace(reg, "");
   }
   else{
       return str;
   }
}
```
7. 已知获取了部分html（截取自码蜂社官网，为minify以后的代码），完成函数getInfo(html)
