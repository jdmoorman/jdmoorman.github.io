* {% if publication.authors %}{% for name in publication.authors %}{% include author_name_link.md %}, {% endfor %}<br>{% endif %}“{% if publication.url %}[*{{ publication.title }}*]({{ publication.url }}){% else %}*{{ publication.title }}*{% endif %}."<br>{{ publication.venue }}