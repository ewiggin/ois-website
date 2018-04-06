---
title: Actualitat
date: 2018-04-06 18:13:00 +01:00
layout: default
---
<div class="row gray full-width page-header vertical-align-table">
    <div class="row full-width padding-top-bottom-50 vertical-align-cell">
        <div class="row">
            <div class="page-header-left">
                <h1>ACTUALITAT</h1>
            </div>
            <div class="page-header-right">
                <div class="bread-crumb-container">
                    <label>Ets aquí:</label>
                    <ul class="bread-crumb">
                        <li>
                            <a title="HOME" href="/">
                                INICI
                            </a>
                        </li>
                        <li class="separator">
                            /
                        </li>
                        <li>
                            ACTUALITAT
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
<div class="clearfix">
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
                    <div class="description t1">
                        {{ post.excerpt }}
                    </div>
                    <div class="row padding-top-54 padding-bottom-17">
                        <a class="more" href="{{post.url}}" title="LLEGIR MÉS">LLEGIR MÉS</a>
                    </div>
                </div>
            </li>
            {% endfor %}
        </ul>
    </div>
</div>