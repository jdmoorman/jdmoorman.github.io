###### Notes

{% for notes in site.teaching %}
{% if notes.layout == 'course_notes' %}
{% if notes.quarter == page.quarter %}
{% if notes.number == page.number %}

* [Week {{ notes.week }}]({{ site.baseurl }}{{ notes.url }})

{% endif %}
{% endif %}
{% endif %}
{% endfor %}