---
title: Tags
---
{% comment %}based on https://github.com/mushishi78/jekyll-group-by-array{% endcomment %}

{% include group-by-array.html collection=site.documents field='tags' %}

{% for tag in group_names %}
{% assign posts = group_items[forloop.index0] %}

<h3 class="tag-heading" id="{{ tag }}">{{ tag }}</h3>
<ul>
    {% for post in posts %}
    <li>
        <a href='{{ site.baseurl }}{{ post.url }}'>{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>
{% endfor %}