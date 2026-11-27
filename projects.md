---
layout: page
title: Projects
permalink: /index.html
---

<div class="posts">
{% for p in site.data.projects %}
<div class="post project">
  <img class="project-image" src="{{ site.baseurl }}{{ p.image }}" alt="{{ p.image_alt }}">
  <div class="project-text">
    <h2>{{ p.title }}</h2>
    <p>{{ p.description }}</p>
    <p class="project-links">
      {% for l in p.links %}<a href="{{ l.url }}">{{ l.label }}</a>{% endfor %}
    </p>
  </div>
</div>
{% endfor %}
</div>
