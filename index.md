---
layout: home
permalink: /
title: ""
---

<div class="container">
  <div class="hero">
    <div class="hero__bio">
      <h1 class="hero__name">Edoardo Carroccetto</h1>
      <p class="hero__role">Data Scientist · Turin</p>

      <p>
        Mathematician and statistician with a strong foundation in <strong>stochastic processes,
        dynamical systems, and statistical inference</strong>, moving into computational neuroscience.
        Particularly interested in the mathematical modelling of brain dynamics and its clinical
        applications to neurological and neurodegenerative conditions.
      </p>

      <p>
        I obtained my MSc in <strong>Stochastics &amp; Data Science</strong> from the University of Turin,
        where my thesis developed asymptotic theory for nonparametric estimators of survival curves
        and quantile treatment effects under right-censoring.
        I spent an exchange semester at <strong>Ghent University</strong> under the supervision of
        Stijn Vansteelandt, deepening my interest in semiparametric and causal methods.
        I currently work as a Data Scientist at <strong>Italdesign</strong> in Turin.
      </p>

      <p>
        Outside of research, I play chess obsessively, run whenever I can, and spend long weekends
        on hiking trails — preferably somewhere with a mountain at the end.
        I also like to travel and keep a small archive of the places I've been, which you can find
        <a href="/travels/" style="border-bottom: 1px solid #dedad1; padding-bottom: 1px;">here</a>.
      </p>

      <div class="hero__links">
        <a class="hero__link" href="{{ site.author.googlescholar }}" target="_blank" rel="noopener">Google Scholar</a>
        <span class="hero__link-sep">·</span>
        <a class="hero__link" href="{{ site.author.orcid }}" target="_blank" rel="noopener">ORCID</a>
        <span class="hero__link-sep">·</span>
        <a class="hero__link" href="https://github.com/{{ site.author.github }}" target="_blank" rel="noopener">GitHub</a>
        <span class="hero__link-sep">·</span>
        <a class="hero__link" href="mailto:{{ site.author.email }}">Email</a>
      </div>
    </div>

    <div class="hero__photo">
      <img src="{{ site.author.avatar | relative_url }}" alt="{{ site.author.name }}">
    </div>
  </div>
</div>

<hr class="divider">

<div class="container">
  <div class="tags">
    <h3>Research interests</h3>
    <div class="tags__list">
      <span class="tags__item">Causal inference</span>
      <span class="tags__item">Survival analysis</span>
      <span class="tags__item">Semiparametric theory</span>
      <span class="tags__item">Stochastic processes</span>
      <span class="tags__item">Computational neuroscience</span>
      <span class="tags__item">Dynamical systems</span>
      <span class="tags__item">Mean-field theory</span>
      <span class="tags__item">Explainable AI</span>
    </div>
  </div>
</div>

<hr class="divider">

<div class="container">
  <div class="pub-list">
    <h3 class="pub-list__heading">Recent publications &amp; projects</h3>

    {% assign recent_pubs = site.publications | sort: 'year' | reverse | limit: 3 %}
    {% for pub in recent_pubs %}
    <div class="pub-item">
      <div>
        <p class="pub-item__title">
          <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a>
        </p>
        <p class="pub-item__meta">{{ pub.year }}{% if pub.authors %} · {{ pub.authors }}{% endif %}</p>
      </div>
      <p class="pub-item__venue">{{ pub.venue }}</p>
    </div>
    {% endfor %}

    {% assign recent_proj = site.projects | sort: 'year' | reverse | limit: 2 %}
    {% for proj in recent_proj %}
    <div class="pub-item">
      <div>
        <p class="pub-item__title">
          <a href="{{ proj.url | relative_url }}">{{ proj.title }}</a>
        </p>
        <p class="pub-item__meta">{{ proj.year }}</p>
      </div>
      <p class="pub-item__venue">{{ proj.category | default: "Project" }}</p>
    </div>
    {% endfor %}
  </div>
</div>
