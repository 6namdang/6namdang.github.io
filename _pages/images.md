---
layout: page
permalink: /images/
title: images
description: Group pictures.
nav: true
nav_order: 4
---

<div class="images-gallery">
  {% for event in site.data.images %}
    <section class="image-section">
      <h2 class="image-section-title">{{ event.period }}</h2>
      {% if event.caption %}
        <p class="image-caption">{{ event.caption }}</p>
      {% endif %}
      {% for image in event.images %}
        <p class="image-frame">
          <a href="{{ image | relative_url }}" title="View full size">
            <img
              src="{{ image | relative_url }}"
              alt="{{ event.period }}"
              loading="lazy"
            >
          </a>
        </p>
      {% endfor %}
    </section>
  {% endfor %}
</div>

<style>
  .images-gallery .image-section {
    margin-bottom: 2.5rem;
  }

  .images-gallery .image-section-title {
    font-size: 1.25rem;
    font-weight: 700;
    margin: 2.5rem 0 1rem;
  }

  .images-gallery .image-section:first-child .image-section-title {
    margin-top: 0;
  }

  .images-gallery .image-caption {
    margin: 0 0 1.25rem;
    line-height: 1.6;
  }

  .images-gallery .image-frame {
    text-align: center;
    margin: 0 0 1.5rem;
  }

  .images-gallery .image-frame:last-child {
    margin-bottom: 0;
  }

  .images-gallery .image-frame img {
    display: inline-block;
    width: auto;
    max-width: 100%;
    height: auto;
    border: 0;
  }

  .images-gallery .image-frame a {
    display: inline-block;
    max-width: 100%;
  }
</style>
