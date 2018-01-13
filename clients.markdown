---
title: Els nostres clients
date: 2017-02-24 13:13:00 +01:00
layout: default
---

<div class="row gray full-width page-padding-top-section padding-bottom-66">
  <div class="row">
    <h2 class="box-header">ELS NOTRES CLIENTS</h2>
    <div class="our-clients-list-container page-margin-top">
      <div class="caroufredsel_wrapper">
        <ul class="our-clients-list">
        {% for item in site.clients %}
          <li>
            <img src="{{item.image}}" alt="{{item.title}}">
          </li>
        {% endfor %}
        </ul>
      </div>
      <div class="re-carousel-pagination" style="display: block;"><a href="#" class="selected"><span>1</span></a><a href="#"><span>2</span></a></div>
    </div>
  </div>
</div>
