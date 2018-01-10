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
				<li><a class="selected" href="/projectes#filter-*" title="All Projects">All Projects</a></li>
				<li><a href="/projectes#filter-renovation" title="Renovation">Renovation</a></li>
				<li><a href="/projectes#filter-design-and-build" title="Design and Build">Design and Build</a></li>
				<li><a href="/projectes#filter-painting" title="Painting">Painting</a></li>
				<li><a href="/projectes#filter-pavers" title="Pavers">Pavers</a></li>
				<li><a href="/projectes#filter-solar-systems" title="Solar Systems">Solar Systems</a></li>
			</ul>
			<ul class="projects-list isotope" style="position: relative; height: 630px;">
        {% for item in site.projects %}
          <li class="pavers" style="position: absolute; left: 300px; top: 0px;">
            <a href="{{item.url}}" title="{{ item.title }}">
              <img src="{{item.image}}" alt="">
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
				<!--<li class="pavers" style="position: absolute; left: 300px; top: 0px;">
					<a href="index.html%3Fpage=project_garden_renovation.html" title="Garden Renovation">
						<img src="/assets/images/samples/270x180/image_04.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Garden Renovation</p>
								<a class="more simple" href="index.html%3Fpage=project_garden_renovation.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="design-and-build painting" style="position: absolute; left: 600px; top: 0px;">
					<a href="index.html%3Fpage=project_painting.html" title="Painting">
						<img src="/assets/images/samples/270x180/image_07.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Painting</p>
								<a class="more simple" href="index.html%3Fpage=project_painting.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="renovation design-and-build" style="position: absolute; left: 0px; top: 210px;">
					<a href="index.html%3Fpage=project_design_build.html" title="Design and Build">
						<img src="/assets/images/samples/270x180/image_10.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Design and Build</p>
								<a class="more simple" href="index.html%3Fpage=project_design_build.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="design-and-build solar-systems" style="position: absolute; left: 300px; top: 210px;">
					<a href="index.html%3Fpage=project_design_build.html" title="Design and Build">
						<img src="/assets/images/samples/270x180/image_08.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Design and Build</p>
								<a class="more simple" href="index.html%3Fpage=project_design_build.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="renovation" style="position: absolute; left: 600px; top: 210px;">
					<a href="index.html%3Fpage=project_interior_renovation.html" title="Interior Renovation">
						<img src="/assets/images/samples/270x180/image_05.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Interior Renovation</p>
								<a class="more simple" href="index.html%3Fpage=project_interior_renovation.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="renovation painting" style="position: absolute; left: 0px; top: 420px;">
					<a href="index.html%3Fpage=project_painting.html" title="Painting">
						<img src="/assets/images/samples/270x180/image_09.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Painting</p>
								<a class="more simple" href="index.html%3Fpage=project_painting.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>
				<li class="solar-systems" style="position: absolute; left: 300px; top: 420px;">
					<a href="index.html%3Fpage=project_solar_systems.html" title="Solar Systems">
						<img src="/assets/images/samples/270x180/image_06.jpg" alt="">
					</a>
					<div class="view align-center">
						<div class="vertical-align-table">
							<div class="vertical-align-cell">
								<p class="description">Solar Systems</p>
								<a class="more simple" href="index.html%3Fpage=project_solar_systems.html" title="VIEW PROJECT">VIEW PROJECT</a>
							</div>
						</div>
					</div>
				</li>-->
			</ul>
		</div>
	</div>
</div>
