---
layout: page
title: Projects
mathjax: true
---

{% for project in site.projects reversed %}
  <div class="project-card">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p class="meta">{{ project.date | date: "%B %Y" }}</p>
    {{ project.excerpt | markdownify }}
    <a href="{{ project.url }}" class="btn">Read More</a>
  </div>
{% endfor %}
