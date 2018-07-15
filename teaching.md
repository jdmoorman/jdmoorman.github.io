---
layout: page
title: Teaching
---

###### Current Courses
{% for course in site.teaching reversed %}
{% if course.layout == 'course_info' %}
{% if course.quarter == site.quarter %}

* [{% include course_listing.md %}]({{ site.baseurl }}{{ course.url }})
{% endif %}

{% endif %}
{% endfor %}

###### Past Courses
{% for course in site.teaching reversed %}
{% if course.quarter != site.quarter %}
{% if course.layout == 'course_info' %}
{% if course.no_link %}
* {% include course_listing.md %}
{% else %}
* [{% include course_listing.md %}]({{ site.baseurl }}{{ course.url }})
{% endif %}
{% endif %}
{% endif %}
{% endfor %}