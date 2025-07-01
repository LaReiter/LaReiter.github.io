---
layout: page
title: Projects
---

Here you can find my selected machine learning and data science projects.

{% for post in site.posts %}
  {% if post.path contains 'projects/' %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
  <p>{{ post.excerpt }}</p>
  <hr>
  {% endif %}
{% endfor %}
