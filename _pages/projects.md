---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<style>

/* PALETTE MULTICOLORE IN ARMONIA */
:root {
  --card-color-1: #e8f5e9; /* Sage */
  --card-color-2: #e9edc9; /* Sand */
  --card-color-3: #d0efd3; /* Soft Mint */
  --card-color-4: #b9cbb8; /* Moss */ 
  --card-color-5: #a3b18a; /* Olive */
  --card-color-6: #cfe8cc; /* Fern Light */
  --card-color-7: #d9ead3; /* Pale Green */
}

/* Layout */
.projects-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
}

/* Wrapper per rendere la card cliccabile */
.project-link-wrapper {
  text-decoration: none;
  color: inherit;
  display: block;
}

.project-card {
  position: relative;
  border-left: 6px solid #2e7d32;
  border-radius: 12px;
  padding: 20px;
  transition: transform 0.3s, box-shadow 0.3s;
}

/* Hover generale */
.project-link-wrapper:hover .project-card {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 12px 25px rgba(0,0,0,0.15);
}

.project-card h3 {
  margin: 0 0 10px 0;
  color: #1b5e20;
  font-size: 1.35em;
}

.project-card p {
  margin: 0 0 12px 0;
  color: #333;
}

/* Tags */
.project-tags {
  margin-top: 10px;
}

.project-tag {
  display: inline-block;
  background: #2e7d32;
  color: #e8f5e9;
  border-radius: 12px;
  padding: 5px 12px;
  font-size: 0.85em;
  margin: 0 5px 5px 0;
  transition: background 0.3s, transform 0.2s;
}

.project-tag:hover {
  background: #1b5e20;
  transform: translateY(-2px);
}
</style>

A selection of projects combining machine learning, statistical modelling, and explainability.

<div class="projects-container">

{% assign colors = "var(--card-color-1),var(--card-color-2),var(--card-color-3),var(--card-color-4),var(--card-color-5),var(--card-color-6),var(--card-color-7)" | split: "," %}

{% for project in site.projects %}
  {% assign index = forloop.index0 | modulo: colors.size %}
  {% assign thiscolor = colors[index] %}
  
  <a class="project-link-wrapper" href="{{ project.url | relative_url }}">
    <div class="project-card" style="background: {{ thiscolor }};">
      <h3>{{ project.title }}</h3>
      <p>{{ project.excerpt }}</p>

      {% if project.tags %}
        <div class="project-tags">
          {% for tag in project.tags %}
            <span class="project-tag">{{ tag }}</span>
          {% endfor %}
        </div>
      {% endif %}
    </div>
  </a>
{% endfor %}
</div>

{% endfor %}
</div>

