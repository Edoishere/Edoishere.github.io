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
  --color-1: #e8f5e9;
  --color-2: #f1f8e9;
  --color-3: #f9fbe7;
  --color-4: #e0f2f1;
  --color-5: #e3f2fd;
  --color-6: #ede7f6;
  --color-7: #fff3e0;

  --border-green: #1b5e20;
  --title-green: #2e7d32;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 25px;
  margin-top: 30px;
}

.project-card {
  border-left: 5px solid var(--border-green);
  border-radius: 10px;
  padding: 20px;
  background: var(--dynamic-color);
  text-decoration: none;
  display: block;
  color: inherit;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.15);
}

.project-card h3 {
  margin-top: 0;
  color: var(--title-green);
}
</style>
{% endraw %}

# Projects

A selection of the projects I’ve worked on, combining machine learning,
statistical mod

