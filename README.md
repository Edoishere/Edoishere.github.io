# edoishere.github.io

Personal academic website — Jekyll, zero theme dependencies.

## Setup locale

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Poi apri `http://localhost:4000`.

## Struttura

```
_config.yml          → configurazione sito (nome, link, nav)
_pages/
  about.md           → homepage
  projects.md        → pagina progetti
  publications.md    → pagina pubblicazioni
  cv.md              → curriculum vitae
_projects/           → un file .md per progetto
_publications/       → un file .md per pubblicazione
images/              → foto profilo (Edo.jpg) e altre immagini
files/               → CV in PDF e altri allegati
_sass/main.scss      → tutto il CSS, scritto da zero
_layouts/            → template HTML
_includes/           → nav, footer, head
```

## Aggiungere una pubblicazione

Crea `_publications/ANNO-titolo-breve.md`:

```yaml
---
title: "Titolo della pubblicazione"
authors: "Carroccetto E., et al."
venue: "Nome rivista o conferenza"
year: 2024
pdf: "/files/paper.pdf"
doi: "10.xxxx/xxxxx"
code: "https://github.com/..."
---

Abstract o descrizione.
```

## Aggiungere un progetto

Crea `_projects/ANNO-nome.md`:

```yaml
---
title: "Nome progetto"
description: "Breve descrizione."
year: 2024
category: "Machine Learning"
tags:
  - Python
  - Causal Inference
github: "https://github.com/Edoishere/..."
---
```

## Deploy

Push su `master` → GitHub Pages builda automaticamente.  
Assicurati che nelle impostazioni del repo sia selezionato **Source: Deploy from branch → master**.
