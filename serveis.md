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
			<!--<ul class="services-list services-icons services-items-border row clearfix margin-top-30">
				<li>
					<a href="index.html%3Fpage=service_tiling_painting.html" title="Tiling and Painting"><span class="service-icon sl-small-bucket"></span></a>
					<div class="service-content">
						<h4 class="box-header"><a href="index.html%3Fpage=service_tiling_painting.html" title="Tiling and Painting">TILING AND PAINTING</a></h4>
						<p>We offer quality tiling and painting solutions for interior and exterior.</p>
					</div>
				</li>
				<li>
					<a href="index.html%3Fpage=service_paver_walkways.html" title="Paver Walkways">
						<span class="service-icon sl-small-bricks"></span>
					</a>
					<div class="service-content">
						<h4 class="box-header"><a href="index.html%3Fpage=service_paver_walkways.html" title="Paver Walkways">PAVER WALKWAYS</a></h4>
						<p>Brick pavers define beauty, elegance and durability for driveways, patios and walkways.</p>
					</div>
				</li>
			</ul>
			<ul class="services-list services-icons services-items-border row clearfix margin-top-30">
				<li>
					<a href="index.html%3Fpage=service_household_repairs.html" title="Household Repairs">
						<span class="service-icon sl-small-wrench"></span>
					</a>
					<div class="service-content">
						<h4 class="box-header"><a href="index.html%3Fpage=service_household_repairs.html" title="Household Repairs">HOUSEHOLD REPAIRS</a></h4>
						<p>We offer affordable and reliable repairs and improvements to the home.</p>
					</div>
				</li>
				<li>
					<a href="index.html%3Fpage=service_solar_systems.html" title="Solar Systems">
						<span class="service-icon sl-small-eco"></span>
					</a>
					<div class="service-content">
						<h4 class="box-header"><a href="index.html%3Fpage=service_solar_systems.html" title="Solar Systems">SOLAR SYSTEMS</a></h4>
						<p>Generate cheap, green electricity from sunlight using photovoltaic cells.</p>
					</div>
				</li>
			</ul>-->
		</div>
	</div>
</div>
