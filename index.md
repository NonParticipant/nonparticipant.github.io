---
title: "Home"
---

# Welcome to {{ site.title }}

{{ site.description }}

## Current Posts

<ul>
{% for post in site.posts %}
  <li>{{ post.date  | date: "%Y-%m-%d" }} - <a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
{% endfor %}
</ul>