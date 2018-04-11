---
layout: page
---

<div class="courses">
  {% for course in site.teaching reversed %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ course.url }}">{{ course.title }}</a></h1>
<!-- 
      <div class="entry">
        {{ course.excerpt }}
      </div> -->

      <!-- <a href="{{ site.baseurl }}{{ course.url }}" class="read-more">Read More</a> -->
    </article>
  {% endfor %}
</div>