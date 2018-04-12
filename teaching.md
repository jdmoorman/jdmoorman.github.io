---
layout: page
---

###### Current Courses
{% for course in site.teaching reversed %}
{% if course.layout == 'course_info' %}

{% capture course_listing %}{{ course.quarter }}, {{ course.number }}, {{ course.name }}{% endcapture %}

{% if course.quarter == site.quarter %}
* [{{ course_listing }}]({{ site.baseurl }}{{ course.url }})
{% endif %}

{% endif %}
{% endfor %}

###### Past Courses
{% for course in site.teaching reversed %}
{% if course.layout == 'course_info' %}

{% capture course_listing %}{{ course.quarter }}, {{ course.number }}, {{ course.name }}{% endcapture %}

{% if course.quarter != site.quarter %}
* {{ course_listing }}
{% endif %}

{% endif %}
{% endfor %}