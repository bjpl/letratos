---
layout: default
title: Photography
---

<div class="photography-index">
  <div class="collection-page">
    <h1>Photography</h1>
    <p class="collection-intro">Recent Photos</p>
  </div>
  
  {% if site.photography.size > 0 %}
  <div class="photography-grid">
    {% for photo in site.photography %}
    <a href="{{ photo.url | relative_url }}" class="photo-tile">
      {% if photo.thumbnail %}
      <img src="{{ photo.thumbnail | relative_url }}" alt="{{ photo.title }}">
      {% elsif photo.images and photo.images.size > 0 %}
      <img src="{{ photo.images[0].url | relative_url }}" alt="{{ photo.title }}">
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
  {% endif %}
</div>