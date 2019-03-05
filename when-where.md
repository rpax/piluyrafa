---
splash_title: Lo importante
splash_subtitle: Cu&aacute;ndo y d&oacute;nde
title: Cu&aacute;ndo y d&oacute;nde
layout: default
group: navigation
---
<div id="fh5co-when-where" class="fh5co-section-gray">
    <div class="container">
        <div class="row">
            <div class="col-md-8 col-md-offset-2 text-center heading-section animate-box">
                <h2>{{ page.title }}</h2>
            </div>
        </div>
        {% for event in site.events %}
            <div class="col-md-6 text-center animate-box">
                <div class="wedding-events">
                    <div class="ceremony-bg" style="background-image: url({{event.image | relative_url }});"></div>
                    <div class="desc">
                        <h3>{{event.title}}</h3>
                        <p><strong>{{event.when}}: {{event.where}}</strong></p>
                        <p>{{ event.content | markdownify }}</p>
                    </div>
                </div>
            </div>
        {% endfor %}
        <div class="row">
            <div class="col-md-12">
                <div id="map" class="fh5co-map"></div>
            </div>
        </div>
    </div>
</div>