---
layout: default
permalink: /projects/
title: Projects
---

<div class="container">
  <header class="page-header">
    <h1>Projects</h1>
  </header>

  <div class="project-grid">
    {% assign sorted_projects = site.projects | sort: 'year' | reverse %}
    {% for project in sorted_projects %}
    <div class="project-card">
      <span class="project-card__year">{{ project.year }}</span>
      <p class="project-card__title">{{ project.title }}</p>
      <p class="project-card__desc">{{ project.description }}</p>
      {% if project.tags %}
      <div class="project-card__tags">
        {% for tag in project.tags %}
        <span class="project-card__tag">{{ tag }}</span>
        {% endfor %}
      </div>
      {% endif %}
      {% if project.github %}
      <a class="project-card__link" href="{{ project.github }}" target="_blank" rel="noopener">GitHub ↗</a>
      {% endif %}
    </div>
    {% endfor %}
  </div>
</div>
