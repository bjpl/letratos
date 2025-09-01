---
layout: default
title: Experimental
---

<div class="collection-page">
  <h1>Experimental Pieces</h1>
  <p style="text-align: center; color: #7f8c8d; margin: 2rem 0;">HTML-based artistic explorations coming soon.</p>
  
  {% if site.experimental.size > 0 %}
  <ul class="poem-list">
    {% for piece in site.experimental %}
    <li>
      <a href="{{ piece.url | relative_url }}">
        <h2 class="poem-list-title">{{ piece.title }}</h2>
        {% if piece.description %}
        <p class="poem-list-meta">{{ piece.description }}</p>
        {% endif %}
      </a>
    </li>
    {% endfor %}
  </ul>
  {% endif %}
</div>