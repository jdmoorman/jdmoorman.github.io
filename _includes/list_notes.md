###### Notes

{% for notes in site.teaching reversed %}
{% if notes.layout == 'course_notes' %}
{% if notes.quarter == page.quarter %}
{% if notes.number == page.number %}

* [Week {{ notes.week }}]({{ site.baseurl }}{{ notes.url }})

{% for topic in notes.topics %}
    * {{ topic }}
{% endfor %}

{% endif %}
{% endif %}
{% endif %}
{% endfor %}