---
title: 'Collection of recipes'
permalink: /index.html
---
Sources provided when recipe is copied or adapted.

## Index 

<ul>
    {% for recipe in site.recipes %}
      <li>
        <a href="{{ recipe.url }}">
          {{ recipe.title }}
        </a>
      </li>
    {% endfor %}
</ul>

## [Tags](/tags)