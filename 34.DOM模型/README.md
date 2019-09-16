###问答题
##### 1. 什么是 Dom？为什么要用 Dom？
DOM是文档对象模型，通过用JavaScript操作DOM模型，可以动态地改变HTML文档。
##### 2. Dom 有哪些常见属性？
常见的属性有：doctype, head, body, activeElement, title, characterSet, cookie, innerText, innerHTML, outerHTML等。
##### 3. 如何设置 Cookie？
通过document.cookie属性即可查看cookie。
##### 4. innerText 和 innerHTML 有什么异同？
innerText返回元素内包含的文本内容，在多层次的时候会按照元素由浅到深的顺序拼接其内容。
innerHTML不是返回元素的文本内容，而是返回元素的HTML结构。
##### 5. innerHTML 和 outerHTML 有什么不同？
innerHTML 返回的内容是其子节点的HTML结构和内容，不包含本身。
outerHTML 返回内容还包括本身的HTML结构。
##### 6. 我们可以使用 document.write() 动态生成文档流吗？如何可以，如何操作？
可以，使用document.write("XXX");
##### 7. 在什么时候，document.write() 会重写文档流？
页面已经渲染完成再调用write方法，它会先调用open方法，擦除当前文档所有内容，然后再写入

---
### 代码题
https://github.com/PangYunsheng8/mfs-homework/blob/master/34.DOM%E6%A8%A1%E5%9E%8B/homework34.html
