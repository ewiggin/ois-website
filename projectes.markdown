---
title: Projectes
date: 2017-02-24 13:13:00 +01:00
layout: default
---

<div class="theme-page padding-bottom-70">
	<div class="row gray full-width page-header vertical-align-table">
		<div class="row full-width padding-top-bottom-50 vertical-align-cell">
			<div class="row">
				<div class="page-header-left">
					<h1>ELS NOSTRES PROJECTES</h1>
				</div>
			</div>
		</div>
	</div>
	<div class="clearfix">
		<div class="row">
			<ul class="tabs-navigation small gray isotope-filters margin-top-70">
				<li><a class="selected" href="{{page.url}}#filter-*" title="TOTS">TOTS</a></li>
        {% for category in site.data.categories %}
          <li>
            <a title="{{ category.name }}" href="{{page.url}}#filter-{{ category.permalink }}">
              {{ category.name }}
            </a>
          </li>
        {% endfor %}
			</ul>
			<ul class="projects-list isotope" style="position: relative; height: 630px;">
        {% for item in site.projectes %}
          <li class="{{item.category}}" style="position: absolute; left: 300px; top: 0px;">
            <a href="{{item.url}}" title="{{ item.title }}">
              <img src="{{item.cover}}" alt="">
            </a>
            <div class="view align-center">
              <div class="vertical-align-table">
                <div class="vertical-align-cell">
                  <p class="description">{{ item.title }}</p>
                  <a class="more simple" href="{{item.url}}" title="DETALLS">DETALLS</a>
                </div>
              </div>
            </div>
          </li>
        {% endfor %}
			</ul>
		</div>
	</div>
</div>
