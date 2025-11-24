---
layout: single
title: "Edoardo Carroccetto"
author_profile: true
---

<style>
/* Container principale */
.profile-container {
  text-align: center;
  padding: 30px;
  font-family: 'Helvetica', sans-serif;
}

/* Titolo principale con effetto gradient */
.profile-container h1 {
  font-size: 3rem;
  background: linear-gradient(90deg, #6a11cb 0%, #2575fc 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* Sezioni */
.section {
  margin-top: 40px;
}

/* Lista delle skill come badge */
.skills {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
  margin-top: 20px;
}

.skill-badge {
  background: linear-gradient(135deg, #ff758c, #ff7eb3);
  color: white;
  padding: 10px 20px;
  border-radius: 30px;
  font-weight: bold;
  transition: transform 0.3s, box-shadow 0.3s;
  cursor: default;
}

.skill-badge:hover {
  transform: scale(1.1);
  box-shadow: 0 10px 20px rgba(0,0,0,0.2);
}

/* Link animati */
a.project-link {
  display: inline-block;
  margin: 10px;
  font-weight: bold;
  color: #2575fc;
  text-decoration: none;
  transition: transform 0.3s, color 0.3s;
}

a.project-link:hover {
  transform: translateY(-3px);
  color: #6a11cb;
}
</style>

<div class="profile-container">

<h1>👋 Hi, I'm Edoardo Carroccetto</h1>

<p>Data Scientist at <strong>Italdesign</strong> | MSc in <em>Stochastics & Data Science</em></p>

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
  <a class="project-link" href="/projects/">🚀 Projects</a>
  <a class="project-link" href="/about/">📖 About Me</a>
</div>

</div>
