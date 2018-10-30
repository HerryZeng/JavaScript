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

