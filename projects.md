---
layout: default
permalink: /projects/
title: Projects
---

<div class="container">
  <header class="page-header">
    <h1>Projects</h1>
  </header>

  <div class="publications-page">
    {% assign proj_by_year = site.projects | sort: 'year' | reverse | group_by: 'year' %}
    {% for year_group in proj_by_year %}
    <div class="pub-year-group">
      <h2>{{ year_group.name }}</h2>
      {% for project in year_group.items %}
      <div class="pub-full-item">
        <div>
          <p class="pub-full-item__title">{{ project.title }}</p>
          {% if project.description %}<p class="pub-full-item__authors">{{ project.description }}</p>{% endif %}
          {% if project.category %}<p class="pub-full-item__venue">{{ project.category }}</p>{% endif %}
          {% if project.tags %}
          <p class="pub-full-item__tags">
            {% for tag in project.tags %}{{ tag }}{% unless forloop.last %} · {% endunless %}{% endfor %}
          </p>
          {% endif %}
        </div>
        <div class="pub-full-item__links">
          {% if project.github %}<a class="pub-full-item__link" href="{{ project.github }}" target="_blank" rel="noopener">GitHub ↗</a>{% endif %}
          {% if project.pdf %}<a class="pub-full-item__link" href="{{ project.pdf }}" target="_blank" rel="noopener">PDF ↗</a>{% endif %}
          {% if project.demo %}<a class="pub-full-item__link" href="{{ project.demo }}" target="_blank" rel="noopener">Demo ↗</a>{% endif %}
        </div>
      </div>
      {% endfor %}
    </div>
    {% endfor %}
  </div>
</div>
