---
layout: page
title: Blog
permalink: /blog/

---

Welcome to my blog! Here you'll find my latest posts about environmental science, research, and field experiences.

<div class="blog-categories">
  <div class="category-section">
    <h2>Environmental Science</h2>
    <p>Articles about environmental science concepts, current issues, and solutions.</p>
    <a href="/blog/environmental-science/" class="category-link">View Environmental Science Posts →</a>
  </div>

  <div class="category-section">
    <h2>Research Updates</h2>
    <p>Updates and insights from my ongoing research projects.</p>
    <a href="/blog/research/" class="category-link">View Research Posts →</a>
  </div>

  <div class="category-section">
    <h2>Field Notes</h2>
    <p>Observations and experiences from field work and data collection.</p>
    <a href="/blog/field-notes/" class="category-link">View Field Notes →</a>
  </div>
</div>

<div class="recent-posts">
  <h2>Recent Posts</h2>
  <div class="post-list">
    {% for post in site.posts limit:5 %}
      <article class="post-item">
        <h3 class="post-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <div class="post-meta">
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
          {% if post.category %}
          <span class="post-category">{{ post.category }}</span>
          {% endif %}
        </div>
        <div class="post-excerpt">
          {{ post.excerpt | strip_html | truncatewords: 50 }}
        </div>
      </article>
    {% endfor %}
  </div>
  
  <div class="view-all">
    <a href="/blog/all/" class="all-posts-link">View All Posts →</a>
  </div>
</div> 