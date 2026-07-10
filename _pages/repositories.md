---
layout: page
permalink: /repositories/
title: repositories
description: GitHub profile and activity for 6namdang.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center mt-4">
    {% include repository/repo_trophies.liquid username=user %}
  </div>
{% endfor %}
{% endif %}

{% endif %}

---

{% include figure.liquid loading="lazy" path="assets/img/kellis-lab-summer-2026.jpg" title="MIT Kellis Lab, RSI Students, and MANTIS AI — Summer 2026" class="img-fluid rounded z-depth-1" %}
<div class="caption">
  Kellis Lab + RSI students + MANTIS AI, Summer 2026.
</div>
