---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<style>
.projects-container {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.project-card {
  position: relative;
  background: #e8f5e9; /* verde chiaro */
  border-left: 6px solid #2e7d32; /* verde scuro */
  border-radius: 10px;
  padding: 20px;
  transition: transform 0.2s, box-shadow 0.2s;
}

.project-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 15px rgba(0,0,0,0.1);
}

.project-card h3 {
  margin: 0 0 8px 0;
  color: #1b5e20; /* verde scuro più profondo */
  font-size: 1.3em;
}

.project-card p {
  margin: 0 0 10px 0;
  color: #333;
}

.project-tags {
  margin-top: 10px;
}

.project-tag {
  display: inline-block;
  background: #2e7d32; /* verde scuro principale */
  color: #e8f5e9; /* verde chiaro testo */
  border-radius: 12px;
  padding: 3px 10px;
  font-size: 0.8em;
  margin-right: 5px;
  margin-bottom: 3px;
  text-decoration: none;
  transition: background 0.2s;
}

.project-tag:hover {
  background: #1b5e20;
}
</style>

A selection of the projects I’ve worked on, combining machine learning, statistical modelling, and explainability.

<div class="projects-container">
{% for project in site.projects %}
  <div class="project-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <p>{{ project.excerpt }}</p>
    {% if project.tags %}
      <div class="project-tags">
        {% for tag in project.tags %}
          <span class="project-tag">{{ tag }}</span>
        {% endfor %}
      </div>
    {% endif %}
  </div>
{% endfor %}
</div>
