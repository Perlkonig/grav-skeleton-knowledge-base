---
title: Authors
redirect: 'taxonomy?name=author'

content:
    items: @self.children

cache_enable: false
twig_first: true
process:
    markdown: false
    twig: true
---

<h1>Authors</h1>
<ul>
{% for p in page.collection %}
    <li><a href="{{ p.url }}">{{ p.title }}</a></li>
{% endfor %}
</ul>

