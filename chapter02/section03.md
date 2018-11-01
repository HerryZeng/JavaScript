## JavaScript HTML DOM - 改变 CSS

---

HTML DOM 允许 JavaScript 改变 HTML 元素的样式。

---

### 改变 HTML 样式
如需改变 HTML 元素的样式，请使用这个语法：
```javascript
document.getElementById(id).style.property=new style
```
例子1
```javascript
<p id="p2">Hello World!</p>

<script>
document.getElementById("p2").style.color="blue";
</script>
```
例子2
```javascript
<h1 id="id1">My Heading 1</h1>

<button type="button" onclick="document.getElementById('id1').style.color='red'">
点击这里
</button>
```
