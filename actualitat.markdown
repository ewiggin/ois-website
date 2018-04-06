---
title: Actualitat
date: 2018-04-06 18:13:00 +01:00
layout: default
---
<div class="row margin-top-70">
    <ul class="blog two-columns clearfix">
        {% for post in site.posts %}
          {% capture thecycle %}{% cycle 'odd', 'even' %}{% endcapture %}
          {% if thecycle == 'odd' %}
            </ul><ul class="blog two-columns clearfix">
          {% endif %}
          <li class="column column-1-2">
            <ul class="post-details">
                <li class="date template-calendar">{{ post.date | date: "%-d %B %Y"  }}</li>
            </ul>
            <div class="post-content">
                <a href="{{post.url}}" title="{{post.title}}" class="post-image">
                    <img src="{{post.image}}" alt="" style="display: block;">
                </a>
                <h3 class="box-header align-left"><a href="{{post.url}}">{{post.title}}</a></h3>
                <p class="description t1">
                    {{ post.excerpt }}
                </p>
                <div class="row padding-top-54 padding-bottom-17">
                    <a class="more" href="{{post.url}}" title="LLEGIR MÉS">LLEGIR MÉS</a>
                </div>
            </div>
          </li>
        {% endfor %}
    </ul>
</div>