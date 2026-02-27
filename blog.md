---
layout: page
title: Blog
permalink: /blog/
---

## EDMT 208 - Online Journal Entries

{% if site.posts.size == 0 %}
No posts yet.
{% endif %}

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%B %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>