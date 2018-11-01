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
例子 2
本例从事件处理器调用一个函数：
```html
<!DOCTYPE html>
<html>
<head>
<script>
function changetext(id)
{
id.innerHTML="谢谢!";
}
</script>
</head>
<body>
<h1 onclick="changetext(this)">请点击该文本</h1>
</body>
</html>
```

---

### HTML 事件属性
如需向 `HTML`元素分配事件，您可以使用事件属性。

实例
向 `button`元素分配 `onclick`事件：
```html
<button onclick="displayDate()">点击这里</button>
```
在上面的例子中，名为 displayDate 的函数将在按钮被点击时执行。

---

### 使用 HTML DOM 来分配事件
HTML DOM 允许您通过使用 JavaScript 来向 HTML 元素分配事件：

实例
向 button 元素分配 onclick 事件：
```javascript
<script>
document.getElementById("myBtn").onclick=function(){displayDate()};
</script>

```
在上面的例子中，名为 displayDate 的函数被分配给 id=myButn" 的 HTML 元素。

当按钮被点击时，会执行该函数。

---

### onload 和 onunload 事件
onload 和 onunload 事件会在用户进入或离开页面时被触发。

onload 事件可用于检测访问者的浏览器类型和浏览器版本，并基于这些信息来加载网页的正确版本。

onload 和 onunload 事件可用于处理 cookie。

实例
```html
<body onload="checkCookies()">
```
