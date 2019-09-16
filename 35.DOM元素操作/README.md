### 问答题
##### 1. dom 元素常用属性有哪些？
1）nodeName：元素标签名
2）nodeType：元素类型
3）className：类名
4）id：元素id
5）children：子元素列表
6）childNodes：子元素列表
7）firstChild：第一个子元素
8）lastChild：最后一个子元素
9）nextSibling：下一个兄弟元素
10）previousSibling：上一个兄弟元素
11）parentNode、parentElement：父元素
##### 2. 如何查找元素？
1）通过id属性查找：getElementById()
2）通过类名查找：getElementsByClassName()
3）通过标签名查找：getElementsByTagName()
4）通过标签的name属性查找：getElementsByName()
5）通过CSS选择器查找：querySelector() querySelectorAll()
6）通过元素在文档中的位置查找：elementFromPoint()
##### 3. 如何增/删/改/查元素？
1）增加元素：
createElement()，createTextNode()，createDocumentFragment()
2）删除元素：
removeChild()
3）修改元素：
appendChild()，insertBefore()，replaceChild()
##### 4. HTMLCollectioin 和 NodeList 有何异同？
相同点：
1）都是类数组对象，都有length属性，可以通过for循环迭代
2）都是只读的
3）都是实时的，即文档的更改会立即反映到相关对象上面
4）有item()方法，可以通过item(index)或item("id")获取元素
不同点：
1）HTMLCollection对象具有namedItem()方法，可以传递id或name获得元素
2）HTMLCollection的item()方法和通过属性获取元素(document.forms.f1)可以支持id和name，而NodeList对象只支持id

---
### 代码题
https://github.com/PangYunsheng8/mfs-homework/blob/master/35.DOM%E5%85%83%E7%B4%A0%E6%93%8D%E4%BD%9C/homework35.html