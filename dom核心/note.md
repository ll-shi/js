# 根据节点获取节点

- **parentNode**：获取父节点（元素、文档）
- previousSibling：获取上一个兄弟节点
- nextSibling：获取下一个兄弟节点
- childNodes：获取所有的子节点
- firstChild：获取第一个子节点
- lastChild：获取最后一个子节点
- attributes: 获取某个元素的属性节点

## 获取元素节点

- parentElement：获取父元素
- previousElementSibling：获取上一个兄弟元素
- nextElementSibling：获取下一个兄弟元素
- children：获取子元素
- firstElementChild：获取第一个子元素
- lastElementChild：获取最后一个子元素

### 获取节点信息

- nodeName：获取节点名称
- nodeValue：获取节点的值
- nodeType：节点类型，是一个数字

### web Api

- BOM：Browser Object Model，浏览器对象模型
- DOM：Document Object Model，文档对象模型

### 节点类型

- DocumentType，文档类型节点
- Document，文档节点，表示整个文档
- Comment，注释节点
- Element，元素节点
- Text，文本节点
- Attribute，属性节点
- DocumentFragment，文档片段节点

### 获取和设置元素属性

- 通用方式：getAttribute、setAttribute

### 阻止浏览器默认行为

dom0的方式：在事件处理程序中返回false

preventDefault方法

阻止事件冒泡：- stopPropagation方法  
