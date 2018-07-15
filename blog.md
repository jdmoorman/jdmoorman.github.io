---
layout: page
title: Blog
---

## Recent

{% for post in site.posts limit: 5%}

* [{{ post.title }}]({{ post.url }}) ({{ post.date | slice: 0, 10}})

{% endfor %}