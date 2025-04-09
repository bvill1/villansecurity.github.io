---
layout: blog
title: Blog
permalink: /blog/
---

Welcome to the Villan Security blog. Here you’ll find long-form thoughts on AI, cybersecurity, decision-making, and critical thinking in tech.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br />
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
