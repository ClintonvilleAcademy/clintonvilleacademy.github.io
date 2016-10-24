---
layout: default
title: {{ site.name }}
---

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    * {{ post.date | date_to_string }} &raquo; [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
  {% endfor %}
{% else %}
  No blog posts yet!
{% endif %}
