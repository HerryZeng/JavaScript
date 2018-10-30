## JavaScript简介

JavaScript是世界上最流行的编程语言。
这门语言可用于`HTML`和`Web`，更可广泛用于服务器，PC，笔记本电脑，平板电脑和智能手机等设备。


### JavaScript是脚本语言

JavaScript是一种轻量级的编程语言。
JavaScript是可插入`HTML`页面的编程代码。
JavaScript插入`HTML`页面后，可由所有的现代浏览器执行。
JavaScript很容易学习。

### 学到什么

在本教程中学到的主要内容。

#### JavaScript:写入HTML输出 

**实例**
```javascript
document.write("<h1>This is a heading</h1>");
document.write("<p>This is a paragraph</p>");
```
提示：只能在`HTML`输出中使用`document.write`，如果在文档加载后使用方法，会覆盖整个文档。

#### JavaScript:对事件作出反应

**实例**
```html
<button type="button" onclick="alert('Welcome!')">占击这里</button>
```
`alert()`函数在JavaScript中并不常用，但它对于代码测试非常方便。
`onclick`事件只是在本教程中学到的众多事件之一。

#### JavaScript:改变HTML内容

使用JavaScript来处理`HTML`内容是非常强大的功能。

**实例**
```html
<p id="demo">JavaScript能改变HTML元素的内容</p>
<script>
    function myFunction() {
    x = document.getElementById("demo") //找到元素
    x.innerHTML = "Hello JavaScript!" //改变内容 
    }
</script>
<button type="button" onclick="myFunction()">占击这里</button>
```
经学会看到`document.getElementByID("some id")`。这个方法是`HTML DOM`中定义的。`DOM`(该当对象模型)是用以访问`HTML`元素的正式W3C标准。

#### JavaScript:改变HTML图像

**实例**
动态地改变`HTML<image>`的来源`src`
```html
		<script type="text/javascript">
			function changeImage(){
				el = document.getElementById("myimage")
				if (el.src.match("bulbon")){
					el.src='img/eg_bulboff.gif'
				}
				else {
					el.src='img/eg_bulbon.gif'
				}
			}
		</script>	
		<img src="img/eg_bulboff.gif" alt="" id="myimage" onclick="changeImage()"/>
		<p>点击灯泡来点亮或熄灭这盏灯</p>
```
JavaScript能够改变任意`HTML`元素的大多数属性，而不仅仅是图片。


#### JavaScript:改变HTML样式

改变`HTML`元素的样式，属于改变`HTML`属性的变种 
```javascript
x=document.getElementById("demo")  //找到元素
x.style.color="#ff0000";           //改变样式
```

#### JavaScript：验证输入

JavaScript常用于验证用户的输入

**实例**
```javascript
if isNaN(x) {alert("Not Numeric")};
```

### 知道吗？

**提示**：JavaScript 与 Java 是两种完全不同的语言，无论在概念还是设计上。

Java（由 Sun 发明）是更复杂的编程语言。

ECMA-262 是 JavaScript 标准的官方名称。

JavaScript 由 Brendan Eich 发明。它于 1995 年出现在 Netscape 中（该浏览器已停止更新），并于 1997 年被 ECMA（一个标准协会）采纳。
