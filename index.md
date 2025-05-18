---
layout: default
---
# Последние записи блога

{% assign recent_posts = site.posts | slice: 0, 10 %}

{% for post in recent_posts %}
## [{{ post.title }}]({{ post.url }})

<small>{{ post.date | date: "%d.%m.%Y" }}</small>

{{ post.excerpt }}

{% endfor %}

[Смотреть все записи]({{ site.baseurl }}/blog/)