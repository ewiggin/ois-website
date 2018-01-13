---
name: Post detail
layout: default
---
<div class="theme-page padding-bottom-66">
	<div class="row gray full-width page-header vertical-align-table">
		<div class="row full-width padding-top-bottom-50 vertical-align-cell">
			<div class="row">
				<div class="page-header-left">
					<h1>ACTUALITAT</h1>
				</div>
				<div class="page-header-right">
					<div class="bread-crumb-container">
						<ul class="bread-crumb">
							<li>
								<a title="BLOG" href="index.html%3Fpage=blog.html">
									ACTUALITAT
								</a>
							</li>
							<li class="separator">
								/
							</li>
							<li>
								{{page.title}}
							</li>
						</ul>
					</div>
				</div>
			</div>
		</div>
	</div>
	<div class="clearfix">
		<div class="row margin-top-70">
			<div class="column column-3-4">
				<div class="blog clearfix">
					<div class="post single">
						<ul class="post-details">
							<li class="date template-calendar">{{page.date}}</li>
						</ul>
						<div class="post-content">
							<a href="#" title="{{page.title}}" class="post-image">
								<img src="{{page.image}}" alt="" style="display: block;">
							</a>
							<ul class="post-content-details clearfix">
								<li>Redacció: <a href="index.html%3Fpage=post.html#" title="Kevin Smith">{{page.author}}</a></li>
							</ul>
							<h2 class="box-header align-left"><a href="#">{{page.title}}</a></h2>
							{{content}}
						</div>
					</div>
				</div>
			</div>
			<div class="column column-1-4 re-smart-column" style="height: 2275px;">
				<div class="re-smart-column-wrapper" style="position: static; bottom: auto; top: auto; width: auto;">
					<h6 class="box-header page-margin-top">Ùltimes entrades</h6>
					<ul class="blog small margin-top-30 clearfix">
            {% for post in site.posts offset: 0 limit: 3  %}
              {% include last_posts.html %}
            {% endfor %}
					</ul>
					<h6 class="box-header page-margin-top">Categories</h6>
					<ul class="taxonomies margin-top-30 clearfix">
						{% for category in site.data.categories %}
              <li>
                <a title="{{ category.name }}" href="/projectes#filter-{{category.permalink}}">
                  {{ category.name }}
                </a>
              </li>
            {% endfor %}
					</ul>
				</div>
			</div>
		</div>
	</div>
</div>
