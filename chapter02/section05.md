## JavaScript HTML DOM 元素（节点）

---

添加和删除节点（HTML 元素）。

---

### 创建新的 HTML 元素

如需向 HTML DOM 添加新元素，您必须首先创建该元素（元素节点），然后向一个已存在的元素追加该元素。
实例
```html
<div id="div1">
<p id="p1">这是一个段落</p>
<p id="p2">这是另一个段落</p>
</div>

<script>
var para=document.createElement("p");
var node=document.createTextNode("这是新段落。");
para.appendChild(node);

var element=document.getElementById("div1");
element.appendChild(para);
</script>
```
例子解释：

这段代码创建新的 `<p>` 元素：
```javascript
var para=document.createElement("p");
```
如需向 `<p>` 元素添加文本，您必须首先创建文本节点。这段代码创建了一个文本节点：
```javascript
var node=document.createTextNode("这是新段落。");
```
然后您必须向 `<p>` 元素追加这个文本节点：

para.appendChild(node);
最后您必须向一个已有的元素追加这个新元素。

这段代码找到一个已有的元素：

var element=document.getElementById("div1");
这段代码向这个已有的元素追加新元素：

element.appendChild(para);

