---
layout: default
permalink: /publications/
title: Publications
---

<div class="container">
  <header class="page-header">
    <h1>Publications</h1>
  </header>

  <div class="publications-page">
    {% assign pubs_by_year = site.publications | sort: 'year' | reverse | group_by: 'year' %}
    {% for year_group in pubs_by_year %}
    <div class="pub-year-group">
      <h2>{{ year_group.name }}</h2>
      {% for pub in year_group.items %}
      <div class="pub-full-item">
        <div>
          <p class="pub-full-item__title">{{ pub.title }}</p>
          {% if pub.authors %}<p class="pub-full-item__authors">{{ pub.authors }}</p>{% endif %}
          {% if pub.venue %}<p class="pub-full-item__venue">{{ pub.venue }}</p>{% endif %}
        </div>
        <div class="pub-full-item__links">
          {% if pub.pdf %}<a class="pub-full-item__link" href="{{ pub.pdf }}" target="_blank">PDF ↗</a>{% endif %}
          {% if pub.doi %}<a class="pub-full-item__link" href="https://doi.org/{{ pub.doi }}" target="_blank">DOI ↗</a>{% endif %}
          {% if pub.code %}<a class="pub-full-item__link" href="{{ pub.code }}" target="_blank">Code ↗</a>{% endif %}
        </div>
      </div>
      {% endfor %}
    </div>
    {% endfor %}
  </div>
</div>
