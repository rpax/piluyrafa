---
splash_title: Lo importante
splash_subtitle: Cu&aacute;ndo y d&oacute;nde
title: Cu&aacute;ndo y d&oacute;nde
layout: titled-page
group: navigation
---
<div class="row row-bottom-padded-md">
{% for event in site.events %}
{% assign subtitle = event.when | append: ': ' | append: event.where %}
{% include _simpleCard.html
    image=event.image
    title=event.title
    subtitle=subtitle
    content=event.content
%}
{% endfor %}
</div>