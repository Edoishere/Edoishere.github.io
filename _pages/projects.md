---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% raw %}
<style>
:root {
  /* Palette principale */
  --violet: #7e57c2;
  --orange: #fb8c00;
  --green: #43a047;
  --mustard: #f1c40f;

  /* Sfondo soft */
  --violet-soft: #f3e5f5;
  --orange-soft: #fff3e0;
  --green-soft: #e8f5e9;
  --mustard-soft: #fff9e6;
}

/* Griglia responsive */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
  gap: 28px;
  margin-top: 30px;
}

/* Card cliccabile */
.project-card {
  padding: 22px;
  border-radius: 12px;
  display: block;
  background: var(--dynamic-bg);
  border-left: 6px solid var(--dynamic-color);
  text-decoration: none; /* rimuove underline */
  color: inherit;
  transition: transform 0.22s ease, box-shadow 0.22s ease;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

/* Titolo */
.project-card h3 {
  margin: 0 0 10px;
  font-weight: 700;
  font-size: 1.25rem;
  color: var(--dynamic-color);
  text-decoration: none; /* rimuove underline */
}

/* Paragrafo */
.project-card p {
  margin: 0;
  color: #333;
  text-decoration: none; /* rimuove underline */
}
</style>
{% endraw %}

A selection of the projects I’ve worked on, combining machine learning,
statistical modelling and explainability.

<div class="projects-grid">

{% assign colors = "violet|orange|green|mustard" | split: "|" %}
{% assign backgrounds = "violet-soft|orange-soft|green-soft|mustard-soft" | split: "|" %}
{% assign index = 0 %}

{% for project in site.projects %}

  {% assign current_color = colors[index] %}
  {% assign current_bg = backgrounds[index] %}

  <a class="project-card"
     href="{{ project.url | relative_url }}"
     style="--dynamic-color: var(--{{ current_color }}); --dynamic-bg: var(--{{ current_bg }});">
      <h3>{{ project.title }}</h3>
      <p>{{ project.excerpt }}</p>
  </a>

  {% assign index = index | plus: 1 %}
  {% if index == colors.size %}
    {% assign index = 0 %}
  {% endif %}

{% endfor %}

</div>


