---
title: Galeria
date: 2017-02-24 13:13:00 +01:00
layout: default
---

<div class="theme-page padding-bottom-70">
    <div class="row gray full-width page-header vertical-align-table">
        <div class="row full-width padding-top-bottom-50 vertical-align-cell">
            <div class="row">
                <div class="page-header-left">
                    <h1>FEINA BEN FETA</h1>
                </div>
                <div class="page-header-right">
                    <div class="bread-crumb-container">
                        <ul class="bread-crumb">
                            <li>
                                <a title="Home" href="index.html%3Fpage=home.html">
                                    INICI
                                </a>
                            </li>
                            <li class="separator">
                                /
                            </li>
                            <li>
                                FEINA BEN FETA
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="clearfix">
        <div class="row">
            <ul id="instafeed" class="services-list clearfix padding-top-70"></ul>
        </div>
    </div>
    <div class="clearfix">
        <div class="row">
            <ul class="services-list clearfix padding-top-70">
                {% for image in site.static_files %}
                    {% if image.path contains 'gallery' %}
                        <li>
                            <a href="{{ site.baseurl }}{{ image.path }}" style="background-image: url('{{ site.baseurl }}{{ image.path }}');" class="prettyPhoto re-preload gallery-item">
                            </a>
                        </li>
                    {% endif %}
                {% endfor %}
            </ul>
        </div>
    </div>
</div>
<script type="text/javascript" src="/assets/js/instafeed.min.js"></script>