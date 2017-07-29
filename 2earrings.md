---
layout: page
title: Серьги
permalink: earrings.html
tags: [серьги из серебра, авторские серьги]
---

Авторские серьги из серебра.

{% for item in site.earrings  %}
  * [![{{ item.title | escape }}]({{ item.thumbnail }}) {{ item.title | escape }}]({{ item.url | relative_url }})
{% endfor %}
