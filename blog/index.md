---
layout: default
title: Blog
permalink: /blog/
---

<section class="page-header">
  <h1>Blog</h1>
  <p>Artykuły o coachingu, celach i praktycznych narzędziach do życia w zgodzie ze sobą.</p>
</section>

<section class="section categories-panel">
  <h2>Kategorie</h2>
  <div class="categories-list">
    {% for category in site.categories %}
      <a class="category-pill" href="/blog/#{{ category[0] | slugify }}">{{ category[0] }} ({{ category[1].size }})</a>
    {% endfor %}
  </div>
</section>

<div class="posts-list">
  {% assign sorted_posts = site.posts | sort: "date" | reverse %}
  {% for post in sorted_posts %}
  <article class="post-card">
    <div class="post-card-top">
      {% if post.categories %}
      <span class="post-category">{{ post.categories | join: ", " }}</span>
      {% endif %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    </div>
    <p class="post-meta">{{ post.date | date: "%d %B %Y" }}</p>
    <p>{{ post.excerpt }}</p>
    <a class="link" href="{{ post.url }}">Czytaj dalej</a>
  </article>
  {% endfor %}
</div>
