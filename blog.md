---
layout: default
title: Blog
permalink: /blog/
---

<section id="main" class="container">
  <header class="major">
    <h2>Blog</h2>
    <p>Reflections on cybersecurity, AI, and the critical thinking needed to navigate both.</p>
  </header>

  <div class="box">
    {% for post in site.posts %}
      <section>
        <header>
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        </header>
        <p>{{ post.excerpt }}</p>
        <ul class="actions">
          <li><a href="{{ post.url }}" class="button small">Read More</a></li>
        </ul>
        <hr />
      </section>
    {% endfor %}
  </div>
</section>
