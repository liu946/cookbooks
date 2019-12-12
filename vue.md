---
layout: cookbook
title:  "Vue"
categories: js
style: compact
---

常见错误
---

- You may have an infinite update loop

> 在模板中使用了子对象函数，写入 methods 再使用即可。

