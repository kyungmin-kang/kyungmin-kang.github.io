---
layout: default
title: Blog
---

<section class="blog-index">
  <h2>📝 Writing</h2>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</section>
