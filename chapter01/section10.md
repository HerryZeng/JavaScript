## JavaScript 函数

---
函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。
实例
```html
<!DOCTYPE html>
<html>
<head>
<script>
function myFunction()
{
alert("Hello World!");
}
</script>
</head>

<body>
<button onclick="myFunction()">点击这里</button>
</body>
</html>
```

---

### JavaScript 函数语法
函数就是包裹在花括号中的代码块，前面使用了关键词 function：
```javascript
function functionname()
{
这里是要执行的代码
}
```
当调用该函数时，会执行函数内的代码。

可以在某事件发生时直接调用函数（比如当用户点击按钮时），并且可由 JavaScript 在任何位置进行调用。

提示：JavaScript 对大小写敏感。关键词 function 必须是小写的，并且必须以与函数名称相同的大小写来调用函数。
