---
layout: default
title: "Blog"
author: "Lars Nørtoft Reiter"
---

{% if site.show_excerpts %}
  {% include home.html %}
{% else %}
  {% include archive.html title="Posts" %}
{% endif %}
