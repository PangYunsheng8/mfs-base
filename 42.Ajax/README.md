### 问答题
##### 1. AJAX 是什么的简称？它和普通的 HTTP 请求有什么不同？
是Asynchronous JavaScript and XML的缩写。它能够向服务器请求额外的数据而无需卸载整个页面。
##### 2. 传统网页的渲染模式和基于 AJAX 的网页渲染模式有何不同？
传统网页在后端将整个网页传至前端，前端可以直接渲染，而基于AJAX的网页后端只会传输需要的数据，前端根据数据修改部分网页内容。
##### 3. 如何模拟调试 AJAX 的数据
使用 Node.js 搭建简易后端来实现Mock数据，Mock数据为后端为前端渲染所需要的返回数据。
##### 4. 如何兼容老浏览器创建 XMLHttpRequest 对象？
```
function createXHR(){
    var xhr = null;
    try {
        // Firefox, Opera 8.0+, Safari，IE7+
        xhr = new XMLHttpRequest();
    }
    catch (e) {
        // Internet Explorer
        try {
            xhr = new ActiveXObject("Msxml2.XMLHTTP");
        }
        catch (e) {
            try {
                xhr = new ActiveXObject("Microsoft.XMLHTTP");
            }
            catch (e) {
                xhr = null;
            }
        }
    }
    return xhr;
}
```
##### 5. XMLHttpRequest 对象有哪几个常用方法？分别对应的含义如何？
1）open方法：open方法规定了要请求的数据的地址以及请求方法。
2）send方法：将请求发往服务器。
##### 6. 常见的 HTTP 请求头有哪些？如何使用 AJAX 设置 HTTP 请求头？
常见的请求头有：
1)Accept：浏览器能够处理的内容类型
2)Accept-Charset：浏览器能够处理的字符集
3)Accept-Encoding：浏览器能够处理的压缩编码
4)Accept-Language：浏览器当前设置的语言
5)Connection：浏览器与服务器的连接类型
6)Cookie：当前页面的cookie
7)Referer:发送请求的页面的URI
可以使用setRequestHeader方法设置自定义的请求Header信息。
##### 7. 如何使用 AJAX 发起 POST 请求？
在open方法第一个参数传入”POST”可以发起POST请求，发起POST请求有时需要传入额外的参数，需要在send方法中传入这些参数。

---
### 代码题
代码：https://github.com/PangYunsheng8/mfs-homework/tree/master/42.Ajax