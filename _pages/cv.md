---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 5
cv_pdf: /assets/pdf/DanielleTsao_CV.pdf
---

<style>
  .post-title,
  h1.post-title,
  .post-header {
    display: none !important;
  }
</style>
 
<div style="max-width: 800px; margin: 0 auto; text-align: center;">
  <a href="{{ page.cv_pdf | relative_url }}" target="_blank" rel="noopener noreferrer"
     style="display: inline-block; padding: 0.6rem 1.5rem; border: 1px solid var(--global-theme-color); border-radius: 4px; color: var(--global-theme-color); text-decoration: none; margin-bottom: 1.5rem;">
    Download CV (PDF)
  </a>
  <div style="width: 100%; height: 85vh; border: 1px solid var(--global-divider-color); border-radius: 4px; overflow: hidden;">
    <embed src="{{ page.cv_pdf | relative_url }}" type="application/pdf" width="100%" height="100%" />
  </div>
</div>
