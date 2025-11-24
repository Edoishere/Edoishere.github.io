---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

# Projects

A selection of the projects I’ve worked on, combining machine learning,
statistical modelling and explainability.

---

{% include base_path %}

{% for project in site.projects %}
- **[{{ project.title }}]({{ project.url | relative_url }})**  
  {{ project.excerpt }}
  <br><br>
{% endfor %}
