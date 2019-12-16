---
layout: cookbook
title:  "Liquid"
categories: 模板引擎
style: compact
---

{% raw %}
对象
---

> 基本语法：`{{ page.title }}`


标记
---

> 基本语法：`{% if user %}`

- 注释 `{% comment %} and {% endcomment %}`
- 赋值 `{% assign tobi = "Tobi" %}`
- 分支 ```
{% if customer.name == 'kevin' %}
  Hey Kevin!
{% elsif customer.name == 'anonymous' %}
  Hey Anonymous!
{% else %}
  Hi Stranger!
{% endif %}
```
- `==`相等, `!=`不相等, `>`大于, `<` 小于
- `>=` 大于或等于, `<=` 小于或等于
- `or` 逻辑或, `and` 逻辑与,
- SWITCH ```
{% case handle %}
  {% when 'cake' %}
     This is a cake
  {% when 'cookie' %}
     This is a cookie
  {% else %}
     This is not a cake nor a cookie
{% endcase %}
```

过滤器
---

> 基本语法：`{{ "/my/fancy/url" | append: ".html" }}` 

{% endraw %}