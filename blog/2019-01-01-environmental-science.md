---
layout: page
title: Environmental Science Blog Posts
permalink: /blog/environmental-science/
---

<div class="category-posts">
  <div class="category-description">
    <h1>Environmental Science</h1>
    <p>Exploring environmental science concepts, current issues, and solutions through in-depth articles and analysis.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts %}
      {% if post.category == "environmental-science" %}
        <article class="post-item">
          <h2 class="post-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>
          <div class="post-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
          </div>
          <div class="post-excerpt">
            {{ post.excerpt | strip_html | truncatewords: 50 }}
          </div>
        </article>
      {% endif %}
    {% endfor %}
  </div>
</div> 