---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

<style>
.projects-timeline {
  position: relative;
  margin: 20px 0 40px 0;
  padding-left: 40px;
}

.projects-timeline::before {
  content: '';
  position: absolute;
  left: 20px;
  top: 0;
  bottom: 0;
  width: 4px;
  background: #2e7d32; /* verde scuro principale */
}

.project-event {
  position: relative;
  margin-bottom: 30px;
  padding-left: 20px;
  background: #e8f5e9; /* verde chiaro */
  border-left: 4px solid #2e7d32;
  border-radius: 8px;
  padding: 15px;
  transition: transform 0.2s, box-shadow 0.2s;
}

.project-event:hover {
  transform: translateY(-3px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.project-event::before {
  content: '';
  position: absolute;
  left: -12px;
  top: 15px;
  width: 16px;
  height: 16px;
  background-color: #2e7d32;
  border-radius: 50%;
  border: 3px solid #e8f5e9;
}

.project-event h4 {
  margin: 0 0 5px 0;
  color: #1b5e20; /* verde scuro più profondo */
}

.project-event p {
  margin: 0;
  color: #333;
}
</style>

# Projects

A selection of the projects I’ve worked on, combining machine learning, statistical modelling, and explainability.

<div class="projects-timeline">
{% for project in site.projects %}
  <div class="project-event">
    <h4><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h4>
    <p>{{ project.excerpt }}</p>
  </div>
{% endfor %}
</div>

