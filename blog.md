---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-content">
  <h2>Blog Posts</h2>
  
  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-item">
        <h3 class="post-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <div class="post-meta">
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
        </div>
        <div class="post-excerpt">
          {{ post.excerpt | strip_html | truncatewords: 50 }}
        </div>
      </article>
    {% endfor %}
  </div>
</div> 