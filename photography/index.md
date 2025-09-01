---
layout: default
title: Photography
---

<div class="collection-page photography-index">
  <h1>Photography</h1>
  <p style="text-align: center; color: #7f8c8d; margin: 2rem 0;">Visual explorations and moments captured in light.</p>
  
  {% if site.photography.size > 0 %}
  <div class="photography-grid">
    {% for photo in site.photography %}
    <a href="{{ photo.url | relative_url }}" class="photo-tile">
      {% if photo.thumbnail %}
      <img src="{{ photo.thumbnail | relative_url }}" alt="{{ photo.title }}" loading="lazy">
      {% elsif photo.images and photo.images.size > 0 %}
      <img src="{{ photo.images[0].url | relative_url }}" alt="{{ photo.title }}" loading="lazy">
      {% endif %}
      <div class="photo-tile-overlay">
        <h2>{{ photo.title }}</h2>
        {% if photo.description %}
        <p>{{ photo.description }}</p>
        {% endif %}
      </div>
    </a>
    {% endfor %}
  </div>
  {% else %}
  <p style="text-align: center; color: #7f8c8d; margin: 3rem 0;">Gallery coming soon.</p>
  {% endif %}
</div>