## JavaScript HTML DOM - 改变 HTML

---

HTML DOM 允许 JavaScript 改变 HTML 元素的内容。


---

### 改变 HTML 输出流

JavaScript 能够创建动态的 `HTML`内容：

今天的日期是： Thu Nov 01 09:58:33 2018 

在 JavaScript 中，`document.write()` 可用于直接向 `HTML`输出流写内容。

实例
```javascript
<!DOCTYPE html>
<html>
<body>

<script>
document.write(Date());
</script>

</body>
</html>
```
提示：绝不要使用在文档加载之后使用 document.write()。这会覆盖该文档。


---

### 改变 HTML 内容
修改 HTML 内容的最简单的方法时使用 innerHTML 属性。

如需改变 HTML 元素的内容，请使用这个语法：
```javascript
document.getElementById(id).innerHTML=new HTML
```
实例
```javascript
<html>
<body>

<p id="p1">Hello World!</p>

<script>
document.getElementById("p1").innerHTML="New text!";
</script>

</body>
</html>
```


---

### 改变 HTML 属性
如需改变 HTML 元素的属性，请使用这个语法：
```javascript
document.getElementById(id).attribute=new value
```
实例
```javascript
<!DOCTYPE html>
<html>
<body>

<img id="image" src="smiley.gif">

<script>
document.getElementById("image").src="landscape.jpg";
</script>

</body>
</html>
```
