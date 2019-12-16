---
layout: cookbook
title:  "CookBook"
style: normal
---

{% comment %}
Linux工具
---
- [Vim](vim.html)


包管理
---
- [Pip Conda](pip_conda.html)


语言
---
- [JS-前端原生](js_origin.html)
- [Vue](vue.html)
- [CSS](css.html)
- [Liquid](liquid.html)

GAME
---
- [MC-WorldEdit](mc_worldedit.html)

{% endcomment %}

{% assign categories = "" %}
{% for cookbook in site.cookbooks  %}
	{% for category in cookbook.categories %}
		{% unless categories contains category %}
			{% assign categories =  category | append: ", " | append: categories %}
		{% endunless %}
	{% endfor %}
{% endfor %}

{% assign categories = categories | split: ", " %}
{% for cur_category in categories %}

{{cur_category}}
---

{% for cookbook in site.cookbooks %}
{% for category in cookbook.categories %}
{% if cur_category == category %}

- [{{ cookbook.title }}]({{ cookbook.url | prepend: site.baseurl }})

{% endif %}
{% endfor %}
{% endfor %}
{% endfor %}




