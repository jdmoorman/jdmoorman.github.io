---
layout: page
title: Presentations
---

{% for presentation in site.slides %}

* [{{ presentation.title }}]({{ site.baseurl }}{{ presentation.url }})

{% endfor %}