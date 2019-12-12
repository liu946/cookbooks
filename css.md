---
layout: cookbook
title:  "CSS"
categories: css
style: compact
---

position
---
- `static` 默认，流式布局，从上到下，从左到右（行内元素）。
- `relative` 流式布局，相对 static原本的位置。只是视觉偏移，其原本站位盒还在原位。
- `absolute` 绝对定位，top, bottom, left, right都可用。`float`失效

> 当祖先中有非`static`的position元素时，根据其进行定位，而不是body。

- `fixed` 绝对定位，相对窗口进行定位。