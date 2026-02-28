---
layout: page
title: Blog
permalink: /blog/
---

## EDMT 208 - Online Journal Entries

{% assign edmt_posts = site.posts | where_exp: "post", "post.course == 'EDMT 208'" %}

{% if edmt_posts.size == 0 %}
No EDMT 208 entries yet.
{% endif %}

<ul>
  {% for post in edmt_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%B %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>

## Beyond the Blackboard

{% assign other_posts = site.posts | where_exp: "post", "post.course != 'EDMT 208'" %}

{% if other_posts.size == 0 %}
No other posts yet.
{% endif %}

<ul>
  {% for post in other_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%B %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>