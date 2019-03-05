---
splash_title: Lo importante
splash_subtitle: Cu&aacute;ndo y d&oacute;nde
title: Cu&aacute;ndo y d&oacute;nde
layout: titled-page
group: navigation
---
<div class="row row-bottom-padded-md">
{% for event in site.events %}
{% include _event.html image=event.image title=event.title when=event.when where=event.where content=event.content %}
{% endfor %}
</div>