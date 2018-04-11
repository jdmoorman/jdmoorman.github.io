---
layout: page
---

<div class="courses">
  {% for course in site.teaching reversed %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ course.url }}">{{ course.title }}</a></h1>
      
    </article>
  {% endfor %}
</div>