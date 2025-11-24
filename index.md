---
layout: single
title: "Edoardo Carroccetto"
author_profile: true
---

{% raw %}
<style>
:root {
  --green-dark: #1b5e20;
  --green-main: #2e7d32;
  --green-light: #e8f5e9;
  --green-soft: #f1f8e9;
  --green-accent: #a5d6a7;
}

/* Container principale */
.profile-container {
  text-align: center;
  padding: 30px;
  font-family: 'Helvetica', sans-serif;
}

/* Titolo principale */
.profile-container h1 {
  font-size: 3rem;
  background: linear-gradient(90deg, var(--green-dark), var(--green-main));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* Sottotitolo */
.profile-container p {
  font-size: 1.2rem;
  color: #444;
}

/* Sezioni */
.section {
  margin-top: 40px;
}

/* Titoli sezione */
.section h2 {
  color: var(--green-main);
  font-weight: 700;
  margin-bottom: 15px;
}

/* Lista delle skill come badge */
.skills {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 12px;
  margin-top: 20px;
}

.skill-badge {
  background: var(--green-light);
  color: var(--green-dark);
  padding: 10px 20px;
  border-radius: 25px;
  font-weight: bold;
  border: 2px solid var(--green-accent);
  transition: transform 0.3s, box-shadow 0.3s;
  cursor: default;
}

.skill-badge:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 14px rgba(0,0,0,0.15);
}

/* Link animati */
a.section-link {
  display: inline-block;
  margin: 10px;
  padding: 12px 22px;
  border-radius: 10px;
  background: var(--green-light);
  border-left: 5px solid var(--green-main);
  color: var(--green-dark);
  font-weight: 600;
  text-decoration: none;
  transition: transform 0.25s, box-shadow 0.25s;
}

a.section-link:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.15);
}

/* Footer spacing */
.footer-space {
  height: 40px;
}
</style>
{% endraw %}

<div class="profile-container">

<h1>👋 Hi, I'm Edoardo Carroccetto</h1>

<p>
  Data Scientist at <strong>Italdesign</strong> · MSc in <em>Stochastics & Data Science</em>  
</p>

<div class="section">
  <h2>💡 My Interests</h2>
  <div class="skills">
    <div class="skill-badge">Computational Psychiatry</div>
    <div class="skill-badge">Cognitive Modelling</div>
    <div class="skill-badge">Reinforcement Learning</div>
    <div class="skill-badge">Causal Machine Learning</div>
    <div class="skill-badge">Survival Analysis</div>
    <div class="skill-badge">Simulation-Based Inference</div>
    <div class="skill-badge">Explainable AI</div>
    <div class="skill-badge">Uncertainty Quantification</div>
  </div>
</div>

<div class="section">
  <h2>📂 Explore My Work</h2>
  <a class="section-link" href="/projects/">🚀 Projects</a>
  <a class="section-link" href="/publications/">📄 Publications</a>
  <a class="section-link" href="/cv/">📘 CV</a>
</div>

<div class="footer-space"></div>

</div>


</div>
