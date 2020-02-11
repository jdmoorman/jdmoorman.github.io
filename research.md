---
layout: page
title: Research
---

I develop algorithms for subgraph matching and analyze randomized iterative methods for solving linear systems.

<!-- ###### Journal Papers

{% for publication in site.data.research.journal %}
{% include publication_item.md %}
{% endfor %} -->

###### Conference Papers

{% for publication in site.data.research.conference %}
{% include publication_item.md %}
{% endfor %}

###### Preprints

{% for publication in site.data.research.preprint %}
{% include publication_item.md %}
{% endfor %}

###### Presentations

{% for publication in site.data.research.presentation %}
{% include publication_item.md %}
{% endfor %}

###### Slides

{% assign presentations = site.slides | sort:"order" | reverse %}
{% for presentation in presentations %}
* [{{ presentation.title }}]({{ site.baseurl }}{{ presentation.url }})
{% endfor %}
