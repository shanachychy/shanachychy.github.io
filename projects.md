---
layout: page
title: Research Projects
mathjax: true
---

## Current Projects

{% for project in site.projects %}
  <div class="project-card">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p class="meta">{{ project.date | date: "%B %Y" }}</p>
    {{ project.excerpt | markdownify }}
    <a href="{{ project.url }}" class="btn">Read More</a>
  </div>
{% endfor %}
