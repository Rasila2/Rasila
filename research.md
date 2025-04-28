---
layout: research
title: Research
permalink: /research/
navID: research
---

Welcome to my research page. Here you'll find information about my research work in environmental science and related fields.

## Research Areas

My research focuses on several key areas:

1. **Climate Change Impact**
   - Himalayan ecosystems
   - Biodiversity changes
   - Water resource management
   - Community adaptation

2. **Biodiversity Conservation**
   - Community-based conservation
   - Protected area management
   - Species monitoring
   - Habitat restoration

3. **Sustainable Development**
   - Mountain communities
   - Renewable energy
   - Eco-tourism
   - Sustainable agriculture

## Current Research Projects

{% for project in site.projects %}
  {% if project.category == "Climate Research" or project.category == "Conservation" %}
    <article class="research-item">
      <h3 class="research-title">
        <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
      </h3>
      <div class="research-meta">
        <time datetime="{{ project.date | date_to_xmlschema }}">{{ project.date | date: "%B %Y" }}</time>
      </div>
      <div class="research-excerpt">
        {{ project.excerpt | markdownify }}
        <a href="{{ project.url | relative_url }}" class="read-more">Read More</a>
      </div>
    </article>
  {% endif %}
{% endfor %}

## Research Methodology

My research approach combines:

- Field studies and observations
- Data analysis and modeling
- Community engagement
- Policy analysis
- Interdisciplinary collaboration

## Publications

A list of my published research papers and articles will be available here soon.

## Collaborations

I welcome opportunities for research collaboration in the following areas:
- Climate change adaptation
- Biodiversity conservation
- Sustainable development
- Community-based research

## Contact

For research inquiries or collaboration opportunities, please feel free to reach out through the contact form or email. 