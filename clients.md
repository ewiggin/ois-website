---
title: Els nostres clients
layout: default 
---

<!-- <div class="row gray full-width page-padding-top-section padding-bottom-66">
  <div class="row">
    <h2 class="box-header">ELS NOTRES CLIENTS</h2>
    <div class="our-clients-list-container page-margin-top">
      <div class="caroufredsel_wrapper">
        <ul class="our-clients-list">
        {% for client in site.clients %}
          <li>
            <img src="{{client.image}}" alt="{{client.title}}"> {{client.title}}
          </li>
        {% endfor %}
        </ul>
      </div>
      <div class="re-carousel-pagination" style="display: block;"><a href="#" class="selected"><span>1</span></a><a href="#"><span>2</span></a></div>
    </div>
  </div>
</div> -->
HOLA..
{% for item in site.clientes %}
  <li>
    <img src="{{item.image}}" alt="{{item.title}}"> {{item.title}}
  </li>
{% endfor %}
