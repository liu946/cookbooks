---
layout: cookbook
title:  "JS-前端原生"
categories: 前端
style: compact
---

DOM树操作
---

- `document.createElement("p")` 新建`p`节点
- `document.createTextNode("这是新段落。")` 新建文本节点
- `document.getElementById("div1")` 查找id节点
- `element.appendChild(para)` 增加子节点
- `parent.removeChild(child)` 删除子节点
- `child.parentNode.removeChild(child)` 删除当前节点

ES6
---

- `[1, 2, 3].reduce((partial_sum, a) => partial_sum + a,0); `