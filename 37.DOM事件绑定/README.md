### 问答题
##### 1. 什么是事件绑定？我们为什么需要它？
事件绑定是指我们可以在事件发生之前，指定事件的响应函数，即告诉计算机当某件事发生时，需要执行哪些代码。
##### 2. 有哪三种方法绑定事件？
1）通过配置HTML元素属性来绑定事件，例如：
```
<div onclick="this.innerHTML='谢谢!'">请点击该文本</div>
```
2）使用DOM指定事件响应函数，例如：
```
document.getElementById("myButton").onclick = myFunction;
```
其中myFunction是事件响应函数。
3）使用 addEventListener() 指定事件响应函数，如：
```
document.getElementById("myButton").addEventListener("click", function(){
  document.getElementById("demo").innerHTML = "Hello World";
});
```
##### 3. document.getElementById("eleID").onclick = onclickHandle 和 addEventListener() 绑定事件处理函数有何异同？不同之处请至少说出3点。
相同点：都可以绑定事件响应函数，当事件发生时，则会执行相应的函数。
不同点：
1）当多个响应函数绑定到同一个事件上时，第一种方法会覆盖掉前面绑定的方法，从而只对最后一个响应函数生效，而第二种方法不会
2）第二种方法可以指定事件是否在捕获或冒泡阶段执行
3）对于 addEventListener 添加的事件，我们可以使用 removeEventListener 删除事件绑定
##### 4. 什么是事件对象？我们如何获取事件对象？
事件对象代表事件的状态，比如事件在其中发生的元素、键盘按键的状态、鼠标的位置、鼠标按钮的状态。在响应函数中加一个事件参数即可获取事件对象。

---
### 代码题
1.预览：https://pangyunsheng8.github.io/mfs-homework/37.DOM%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A/homework37_1.html
代码：https://github.com/PangYunsheng8/mfs-homework/blob/master/37.DOM%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A/homework37_1.html
2.预览：https://pangyunsheng8.github.io/mfs-homework/37.DOM%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A/homework37_2.html
代码：https://github.com/PangYunsheng8/mfs-homework/blob/master/37.DOM%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A/homework37_2.html