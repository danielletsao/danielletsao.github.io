---
layout: page
permalink: /Research/
title: Research
nav: true
sections:
  - heading: "Preprints"
    entries:
      - authors: "D. Tsao, K. Muandet, F. Eberhardt, E. Perković"
        year: "2026"
        title: "Lost in Aggregation: The Causal Interpretation of the IV Estimand"
        links:
          - label: "arxiv"
            url: "https://arxiv.org/abs/2601.12120"
  - heading: "Publications"
    entries:
      - authors: "D. Tsao, R. Perry, C. Cinelli"
        year: "2025"
        title: "On the minimum strength of (unobserved) covariates to overturn an insignificant result"
        venue: "Statistical Science"
        links:
          - label: "arxiv"
            url: "https://arxiv.org/abs/2408.13901"
          # - label: "published version"
          #   url: "To appear in 2026"
      - authors: "X. Ji, D. Tsao, K. Bai, M. Tsao, L. Xing, X. Zhang"
        year: "2023"
        title: "scAnnotate: an automated cell-type annotation tool for single-cell RNA-sequencing data"
        venue: "Bioinformatics Advances"
        links: 
          - label: "arxiv"
            url: "https://www.biorxiv.org/content/10.1101/2022.02.19.481159v1"
          - label: "published version"
            url: "https://doi.org/10.1093/bioadv/vbad030"
---

<!-- _pages/publications.md -->
<style>
  .post-title,
  h1.post-title {
    font-size: 2rem !important;
    margin-bottom: 0.5rem !important;
    font-weight: 400
  }
</style>

<!-- _pages/publications.md -->
<style>
  .post-title,
  h1.post-title,
  .post-header {
    display: none !important;
  }
</style>
<div class="publications">
  <div>
    {% for section in page.sections %}
      <h3 style="font-weight: 400; margin-top: 4rem; margin-bottom: 0.5rem; padding-bottom: 0.75rem; border-bottom: 1px solid var(--global-divider-color);">
        {{ section.heading }}
      </h3>
      <ul style="margin-top: 1rem;">
        {% for entry in section.entries %}
          <li style="margin-bottom: 1.5rem;">
            <div>{{ entry.authors }} ({{ entry.year }}), <strong>{{ entry.title }}</strong>. {% if entry.venue %}<em>{{ entry.venue }}</em>.{% endif %}</div>
            {% if entry.links %}
              <div style="margin-top: 0.4rem;">
                {% for link in entry.links %}(<a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>) {% unless forloop.last %} {% endunless %}{% endfor %}
              </div>
            {% endif %}
          </li>
        {% endfor %}
      </ul>
    {% endfor %}
  </div>
</div>