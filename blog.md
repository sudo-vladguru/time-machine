---
layout: default
title: Все записи
permalink: /blog/
---

# Все записи блога

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

<small>{{ post.date | date: "%d.%m.%Y" }}</small>

{{ post.content }}

---

{% endfor %}

[назад](./)
