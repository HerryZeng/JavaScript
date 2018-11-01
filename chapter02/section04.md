## JavaScript HTML DOM 事件

---

HTML DOM 使 JavaScript 有能力对 HTML 事件做出反应。

---

### 对事件做出反应
我们可以在事件发生时执行 JavaScript，比如当用户在 HTML 元素上点击时。

如需在用户点击某个元素时执行代码，请向一个 HTML 事件属性添加 JavaScript 代码：
```javascript
onclick=JavaScript
```
HTML 事件的例子：
+ 当用户点击鼠标时 
+ 当网页已加载时 
+ 当图像已加载时 
+ 当鼠标移动到元素上时 
+ 当输入字段被改变时 
+ 当提交 HTML 表单时 
+ 当用户触发按键时 

例子 1
在本例中，当用户在 `<h1>` 元素上点击时，会改变其内容：
```javascript
<h1 onclick="this.innerHTML='谢谢!'">请点击该文本</h1>
```