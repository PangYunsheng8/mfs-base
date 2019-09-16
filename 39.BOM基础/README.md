### 问答题
##### 1. BOM 是什么？提供的 API 让我们能操作什么？
BOM是Browser Object Model的缩写，简称浏览器对象模型。BOM提供了一些访问窗口对象的一些方法，我们可以用它来移动窗口位置，改变窗口大小，打开新窗口和关闭窗口，弹出对话框，进行导航以及获取客户的一些信息。
##### 2. window.name 有怎样的特性
就是浏览器刷新后，该属性保持不变。
##### 3. 如何获取窗口的尺寸？
window.innerHeight：获取浏览器窗口的内部高度。
window.innerWidth：获取浏览器窗口的内部宽度。
##### 4. 如何调整滚动条位置
window.scrollTo(x, y)：滚动条移动到(x, y)处。
scrollBy(0, y)：滚动条下移y。
##### 5. 如何获取浏览器相关信息
使用window对象的navigator属性。
##### 6. 如何得到一个元素计算后的属性值
使用window.getComputedStyle方法。
##### 7. 如何模拟点击前进后退按钮的点击？
history.back()：与在浏览器点击后退按钮相同。
history.forward()：与在浏览器中点击按钮向前相同。