## JavaScript 对象

---

JavaScript 中的所有事物都是对象：字符串、数值、数组、函数...

此外，JavaScript 允许自定义对象。

---

### JavaScript 对象
JavaScript 提供多个内建对象，比如 String、Date、Array 等等。

对象只是带有**属性**和**方法**的特殊数据类型。


---

### 方法对象的属性
属性是与对象相关的值。

访问对象属性的语法是：
```javascript
objectName.propertyName
```
这个例子使用了 String 对象的 length 属性来获得字符串的长度：
```javascript
var message="Hello World!";
var x=message.length;
```
在以上代码执行后，x 的值将是：`12`

---

### 方法对象的方法
方法是能够在对象上执行的动作。

您可以通过以下语法来调用方法：
```javascript
objectName.methodName();
```
这个例子使用了 `String`对象的 `toUpperCase()`方法来将文本转换为大写：
```javascript
var message="Hello world!";
var x=message.toUpperCase();
```
在以上代码执行后，x 的值将是：`HELLO WORLD!`

---

### 创建 JavaScript 对象
通过 JavaScript，您能够定义并创建自己的对象。

创建新对象有两种不同的方法：

1. 定义并创建对象的实例 
2. 使用函数来定义对象，然后创建新的对象实例 

