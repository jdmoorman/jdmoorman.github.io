---
layout: page
title: Research
---

I work on developing algorithms for subgraph matching and analyzing randomized iterative methods for solving linear systems.

###### Publications

{% for publication in site.data.publications %}
* {% for name in publication.authors %}{% if name == publication.my_name %}**{{ name }}**{% else %}{{ name }}{% endif %}, {% endfor %}"[*{{ publication.title }}.*]({{ publication.url }})" {{ publication.venue }}.
{% endfor %}

###### Slides

{% for presentation in site.slides %}
* [{{ presentation.title }}]({{ site.baseurl }}{{ presentation.url }})
{% endfor %}
