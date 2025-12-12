---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% raw %}
<style>
/* Stile generale lista progetti */
.project-list {
  list-style-type: none;
  padding-left: 0;
  margin: 0;
}

.project-item {
  background: #f1f8e9; /* verde chiaro */
  border-left: 5px solid #2e7d32; /* verde scuro */
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  transition: transform 0.2s, box-shadow 0.2s;
}

.project-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 12px rgba(0,0,0,0.1);
}

.project-item h3 {
  margin-top: 0;
  color: #1b5e20;
}

.project-item p {
  margin: 8px 0;
  line-height: 1.6;
}

.project-item a {
  color: #2e7d32;
  text-decoration: none;
  font-weight: bold;
}

.project-item a:hover {
  text-decoration: underline;
}

.badge {
  display: inline-block;
  background: #a5d6a7;
  color: #1b5e20;
  padding: 3px 8px;
  border-radius: 12px;
  font-size: 0.85em;
  margin-right: 5px;
}

.section-title {
  border-bottom: 2px solid #2e7d32;
  padding-bottom: 5px;
  margin-top: 40px;
  margin-bottom: 20px;
  color: #2e7d32;
}
</style>
{% endraw %}

# Projects

Here is a selection of my main projects, highlighting my work in data science, machine learning, and computational biology.

<ul class="project-list">
  <li class="project-item">
    <h3>Protein Structure Modelling via Topological Data Analysis</h3>
    <p>
      I applied <span class="badge">Python</span> and <span class="badge">Topological Data Analysis (TDA)</span> to study protein folding and interactions.
      The project explores how TDA can uncover structural patterns not easily detectable with conventional methods, aiming to predict protein functions and stability.
    </p>
    <p>
      <strong>Key contributions:</strong> persistent homology analysis, visualization of protein topologies, and predictive modelling of interaction sites.
    </p>
    <p><strong>Repo:</strong> <a href="#">github.com/Edoishere/protein-tda</a></p>
  </li>

  <li class="project-item">
    <h3>Reinforcement Learning Model for Parkinson-Related Neuronal Function</h3>
    <p>
      Developed a computational model simulating dopamine-dependent decision processes in Parkinson's disease using <span class="badge">Reinforcement Learning</span> and <span class="badge">Python</span>.
      Focused on understanding how neuronal network dynamics are affected and exploring potential strategies for intervention.
    </p>
    <p>
      <strong>Key contributions:</strong> neuron-level RL simulations, reward-based learning, and analysis of dopamine modulation on action selection.
    </p>
    <p><strong>Repo:</strong> <a href="#">github.com/Edoishere/rl-parkinson-neurons</a></p>
  </li>

  <li class="project-item">
    <h3>Revenue Forecasting at Italdesign</h3>
    <p>
      Built an end-to-end forecasting system using <span class="badge">LSTM</span> and <span class="badge">XGBoost</span> to predict company revenues with high accuracy.
      Focused on feature engineering, model evaluation, and time-series forecasting for actionable business insights.
    </p>
    <p>
      <strong>Key contributions:</strong> hybrid ML model design, evaluation metrics comparison, and deployment-ready forecasting pipeline.
    </p>
    <p><strong>Repo:</strong> *(private / placeholder)*</p>
  </li>

  <li class="project-item">
    <h3>Portfolio Clustering at Italdesign</h3>
    <p>
      Applied unsupervised learning techniques to cluster the internal portfolio, enabling strategic segmentation and analysis of revenue streams.
      Used <span class="badge">Python</span> and <span class="badge">scikit-learn</span> to extract meaningful patterns from historical data.
    </p>
    <p>
      <strong>Key contributions:</strong> clustering analysis, data preprocessing, visualization of portfolio segments, and business recommendation insights.
    </p>
    <p><strong>Repo:</strong> *(private / placeholder)*</p>
  </li>
</ul>

<div class="section-title">More Projects</div>

<p>
For additional projects and code samples, please visit my GitHub profile:  
👉 <a href="https://github.com/Edoishere">https://github.com/Edoishere</a>
</p>




