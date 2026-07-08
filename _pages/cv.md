---
layout: page
permalink: /cv/
title: cv
nav: true
nav_order: 5
cv_pdf: /assets/rendercv/rendercv_output/Hoang_Nam_Dang_CV.pdf
description: Research engineer at MIT CSAIL. AI for Science, machine learning, and computer vision.
---

<div class="text-center mb-4">
  <a href="{{ page.cv_pdf | relative_url }}" class="btn btn-primary" target="_blank" rel="noopener noreferrer">
    <i class="fa-solid fa-file-pdf"></i> Download CV (PDF)
  </a>
</div>

<iframe
  src="{{ page.cv_pdf | relative_url }}"
  title="Hoang Nam Dang CV"
  style="border: 0; width: 100%; height: 1100px;"
></iframe>
