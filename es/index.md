---
layout: default
title: Poemas en Español
lang: es
---

<div class="collection-page">
  <h1>Poemas en Español</h1>
  
  <ul class="poem-list">
    {% assign poems = site.poems_es | sort: 'date' | reverse %}
    {% for poem in poems %}
    <li>
      <a href="{{ poem.url | relative_url }}">
        <h2 class="poem-list-title">{{ poem.title }}</h2>
      </a>
    </li>
    {% endfor %}
  </ul>
</div>