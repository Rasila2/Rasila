---
layout: page
title: Projects
permalink: /projects/

---

Explore my projects related to environmental science and research.

<div class="project-content">
  <h2>My Projects</h2>
  
  <div class="project-list">
    {% for projects in site.projects %}
      <article class="project-item">
        <h3 class="project-title">
          <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
        </h3>
        <div class="project-meta">
          <time datetime="{{ project.date | date_to_xmlschema }}">{{ project.date | date: "%B %-d, %Y" }}</time>
        </div>
        <div class="project-excerpt">
          {{ project.excerpt | strip_html | truncatewords: 50 }}
        </div>
      </article>
    {% endfor %}
  </div>
</div> 