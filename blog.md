---
layout: default
title: Blog | KM Kang
---

<section class="blog-list">
  <h2>Writing</h2>
  <p>Essays and reflections on data science, economics, machine learning, and building things.</p>

  <div class="tag-filter">
    <strong>Filter by tag:</strong>
    {% assign tags = site.tags | sort %}
    {% for tag in tags %}
      <a href="#{{ tag[0] }}" class="tag-link">{{ tag[0] }}</a>
    {% endfor %}
  </div>

  <div class="writing-grid">
    {% assign sorted_posts = site.posts | sort: 'date' %}
    {% for post in sorted_posts %}
      <div class="writing-card" id="{{ post.tags[0] }}">
        <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
        <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
        <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
        <div class="tags">
          {% for tag in post.tags %}
          <span>{{ tag }}</span>
          {% endfor %}
        </div>
      </div>
    {% endfor %}
  </div>
</section>

<link rel="stylesheet" href="/assets/css/style.css">
