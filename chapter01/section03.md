## JavaScript使用

HTML 中的脚本必须位于 `<script>` 与 `</script>` 标签之间。

脚本可被放置在 HTML 页面的 `<body>` 和 `<head>` 部分中。

----
### `<script>` 标签
如需在 HTML 页面中插入 JavaScript，请使用 `<script>` 标签。

`<script>` 和 `</script>` 会告诉 JavaScript 在何处开始和结束。

`<script>` 和 `</script>` 之间的代码行包含了 JavaScript：
```javascript
<script>
alert("My First JavaScript");
</script>
```
您无需理解上面的代码。只需明白，浏览器会解释并执行位于 `<script>` 和 `</script>` 之间的 JavaScript。

那些老旧的实例可能会在` <script>` 标签中使用 `type="text/javascript"`。现在已经不必这样做了。JavaScript 是所有现代浏览器以及 HTML5 中的默认脚本语言。

----


### `<body>` 中的 JavaScript
在本例中，JavaScript 会在页面加载时向`HTML`的 `<body>` 写文本：
```html
<!DOCTYPE html>
<html>
<body>
.
.
<script>
document.write("<h1>This is a heading</h1>");
document.write("<p>This is a paragraph</p>");
</script>
.
.
</body>
</html>
```
---

### JavaScript 函数和事件
上面例子中的 JavaScript 语句，会在页面加载时执行。

通常，我们需要在某个事件发生时执行代码，比如当用户点击按钮时。

如果我们把 JavaScript 代码放入函数中，就可以在事件发生时调用该函数。

您将在稍后的章节学到更多有关 JavaScript 函数和事件的知识。

---

### `<head>` 或 `<body>` 中的 JavaScript
您可以在 `HTML`文档中放入不限数量的脚本。

脚本可位于`HTML`的 `<body>` 或 `<head>` 部分中，或者同时存在于两个部分中。

通常的做法是把函数放入 `<head>` 部分中，或者放在页面底部。这样就可以把它们安置到同一处位置，不会干扰页面的内容。

---

### `<head>` 中的 JavaScript 函数
在本例中，我们把一个 JavaScript 函数放置到 `HTML`页面的 `<head>` 部分。

该函数会在点击按钮时被调用：
```html
<!DOCTYPE html>
<html>

<head>
<script>
function myFunction()
{
document.getElementById("demo").innerHTML="My First JavaScript Function";
}
</script>
</head>

<body>

<h1>My Web Page</h1>

<p id="demo">A Paragraph</p>

<button type="button" onclick="myFunction()">Try it</button>

</body>
</html>
```

---

### `<body>` 中的 JavaScript 函数
在本例中，我们把一个 JavaScript 函数放置到 `HTML`页面的 `<body>` 部分。

该函数会在点击按钮时被调用：
```html
<!DOCTYPE html>
<html>
<body>

<h1>My Web Page</h1>

<p id="demo">A Paragraph</p>

<button type="button" onclick="myFunction()">Try it</button>

<script>
function myFunction()
{
document.getElementById("demo").innerHTML="My First JavaScript Function";
}
</script>

</body>
</html>
```





