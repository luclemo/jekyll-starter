---
layout: default
title: "Blog"
permalink: /blog/
nav_order: 3
---

# {{ page.title }}

<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date: "%b %-d, %Y" }}
      <h2><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
    </li>
  {% endfor %}
</ul>