---
layout: default
title: {{ site.name }}
---

{% if site.posts.size > 0 %}
  <ul>
  {% for post in site.posts %}
	<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  </ul>
{% else %}
  No blog posts yet!
{% endif %}
