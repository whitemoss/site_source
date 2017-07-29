---
layout: page
title: Кольца
permalink: rings.html
tags: [кольцо, кольца из серебра, авторские кольца]
---

Авторские кольца из серебра.

{% for item in site.rings %}
  * [![{{ item.title | escape }}]({{ item.thumbnail }}) {{ item.title | escape }}]({{ item.url | relative_url }})
{% endfor %}
