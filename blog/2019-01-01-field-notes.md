---
layout: page
title: Field Notes
permalink: /blog/field-notes/
---

<div class="category-posts">
  <div class="category-description">
    <h1>Field Notes</h1>
    <p>Experience the day-to-day reality of environmental research through field observations, data collection stories, and on-site discoveries.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts %}
      {% if post.category == "field-notes" %}
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