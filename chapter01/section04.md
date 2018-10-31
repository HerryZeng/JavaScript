## JavaScript输出

---

JavaScript通常用于操作`HTML`元素

---

### 操作HTML元素

如果从JavaScript访问某个`HTML`元素，可以使用`document.getElementById(id)`方法。需使用`id`属性来标识`HTML`元素。
例子
通过指定的 id 来访问 HTML 元素，并改变其内容：
```python
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