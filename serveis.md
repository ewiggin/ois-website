---
title: Serveis
date: 2017-02-24 13:13:00 +01:00
layout: default
---

<div class="theme-page padding-bottom-70">
	<div class="row gray full-width page-header vertical-align-table">
		<div class="row full-width padding-top-bottom-50 vertical-align-cell">
			<div class="row">
				<div class="page-header-left">
					<h1>ELS NOSTRES SERVEIS</h1>
				</div>
			</div>
		</div>
	</div>
	<div class="clearfix">
		<div class="row padding-top-70">
			<ul class="services-list services-icons services-items-border row clearfix">
        {% for servei in site.serveis %}
          <li>
            <a href="{{servei.url}}" title="{{servei.name}}">
              <span class="service-icon {{servei.icon}}"></span>
            </a>
            <div class="service-content">
              <h4 class="box-header"><a href="{{servei.url}}" title="{{servei.name}}">{{servei.name}}</a></h4>
              <p>{{servei.claim}}</p>
            </div>
          </li>
        {% endfor %}
			</ul>
		</div>
	</div>
</div>
