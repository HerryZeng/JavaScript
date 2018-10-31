## JavaScript输出

---

JavaScript通常用于操作`HTML`元素

---

### 操作HTML元素

如果从JavaScript访问某个`HTML`元素，可以使用`document.getElementById(id)`方法。需使用`id`属性来标识`HTML`元素。
例子
通过指定的 id 来访问 HTML 元素，并改变其内容：
```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>

<p id="demo">My First Paragraph</p>

<script>
document.getElementById("demo").innerHTML="My First JavaScript";
</script>

</body>
</html>

```
JavaScript 由 web 浏览器来执行。在这种情况下，浏览器将访问 id="demo" 的 HTML 元素，并把它的内容（innerHTML）替换为 "My First JavaScript"。

---

### 写到文档输出
下面的例子直接把 <p> 元素写到 HTML 文档输出中：

实例
```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>

<script>
document.write("<p>My First JavaScript</p>");
</script>

</body>
</html>
```

---

### 警告

请使用 document.write() 仅仅向文档输出写内容。

如果在文档已完成加载后执行 document.write，整个 HTML 页面将被覆盖：

实例
```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>

<p>My First Paragraph.</p>

<button onclick="myFunction()">点击这里</button>

<script>
function myFunction()
{
document.write("糟糕！文档消失了。");
}
</script>

</body>
</html>
```
