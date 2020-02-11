---
layout: page
title: Slides
---

{% assign presentations = site.slides | sort:"order" | reverse %}
{% for presentation in presentations %}
* [{{ presentation.title }}]({{ site.baseurl }}{{ presentation.url }})
{% endfor %}
