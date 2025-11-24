---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<style>
.projects-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
}

/* Link che avvolge la card */
.project-link-wrapper {
  text-decoration: none;      /* rimuove underline */
  color: inherit;             /* mantiene il colore del testo interno */
  display: block;             /* necessario per far sì che l'intera card sia cliccabile */
}

.project-card {
  position: relative;
  background: linear-gradient(145deg, #e8f5e9, #d0efd3); /* verde chiaro sfumato */
  border-left: 6px solid #2e7d32;
  border-radius: 12px;
  padding: 20px;
  transition: transform 0.3s, box-shadow 0.3s, border-color 0.3s;
}

.project-link-wrapper:hover .project-card {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 12px 25px rgba(0,0,0,0.15);
  border-color: #1b5e20;
}

.project-card h3 {
  margin: 0 0 10px 0;
  color: #1b5e20;
  font-size: 1.4em;
}

.project-card p {
  margin: 0 0 12px 0;
  color: #333;
  line-height: 1.5;
}

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
{% for project in site.projects %}
  <a class="project-link-wrapper" href="{{ project.url | relative_url }}">
    <div class="project-card">
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

