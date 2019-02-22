---
layout: page
title: Research
---

I develop algorithms for subgraph matching and analyze randomized iterative methods for solving linear systems.

###### Publications

{% for publication in site.data.publications %}
* {% for name in publication.authors %}{% if name == publication.my_name %}**{{ name }}**{% else %}{{ name }}{% endif %}, {% endfor %}"[*{{ publication.title }}.*]({{ publication.url }})" {{ publication.venue }}
{% endfor %}

###### Slides

{% assign presentations = site.slides | sort:"order" | reverse %}
{% for presentation in presentations %}
* [{{ presentation.title }}]({{ site.baseurl }}{{ presentation.url }})
{% endfor %}
