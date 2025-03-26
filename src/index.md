---
layout: base.html
title: Home
---

# Ray Zilli
a blog about nothing 

{% for post in collections.posts | reverse %}
- [{{ post.data.title }}]({{ post.url }}) - {{ post.date | readableDate }}
{% endfor %}