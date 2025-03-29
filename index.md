---
title: 'Collection of recipes'
permalink: /index.html
---
This is a collection of recipes that I have compiled from various sources including the internet, rednote, newspaper articles and family recipes.

Sources provided when recipe is copied or adapted.

## Index 

<ul>
    {% for recipe in site.recipes %}
      <li>
        <a href="{{ site.baseurl }}{{ recipe.url }}">
          {{ recipe.title }}
        </a>
      </li>
    {% endfor %}
</ul>

## [Tags]({{ site.baseurl }}/tags)