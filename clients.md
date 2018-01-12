---
title: Els nostres clients
layout: default 
---

<div class="row gray full-width page-padding-top-section padding-bottom-66">
  <div class="row">
    <h2 class="box-header">ELS NOTRES CLIENTS</h2>
    <div class="our-clients-list-container page-margin-top">
      <div class="caroufredsel_wrapper" style="display: block; text-align: center; float: none; position: relative; top: auto; right: auto; bottom: auto; left: auto; z-index: 0; width: 1200px; height: 120px; margin: 0px; overflow: hidden;">
        <ul class="our-clients-list re-preloader_0" style="display: block; text-align: left; float: none; position: absolute; top: 0px; right: auto; bottom: auto; left: 0px; margin: 0px; width: 6000px; height: 120px;">
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
