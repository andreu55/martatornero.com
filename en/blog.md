---
layout: default
title: Blog
locale: en
permalink: "/blog/en/"
altlang: /blog/es/
---

## {{ page.title }}

<nav>
  <ul class="posts-list">
    {% for post in site.posts %}
    <li>
      <span class="date">{{ post.date | date: "%F" }}</span>:
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
  </ul>
</nav>
