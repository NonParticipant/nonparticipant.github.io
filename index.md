---
title: "Home"
---

{% assign sections = site.mainpage | sort: 'order' %}

{% for section in sections %}
{% if section.include != null %}
{% include {{ section.include }} %}
{% else %}
{% include sections/default.html %}
{% endif %}
{% endfor %}
