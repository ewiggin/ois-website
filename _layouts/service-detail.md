---
name: Serveis
layout: default
---

<div class="theme-page">
  <div class="row gray full-width page-header vertical-align-table">
    <div class="row full-width padding-top-bottom-50 vertical-align-cell">
      <div class="row">
        <div class="page-header-left">
          <h1>{{page.title}}</h1>
        </div>
        <div class="page-header-right">
          <div class="bread-crumb-container">
            <ul class="bread-crumb">
              <li>
                <a title="{{page.title}}" href="{{page.url}}">
                  ELS NOSTRES SERVEIS
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
      <div class="column column-1-4">
        <ul class="vertical-menu">
          {% for servei in site.serveis %}
            {% if servei.url == page.url %}
              <li class="selected">
                <a href="{{servei.url}}" title="{{servei.name}}">
                  {{servei.name}}
                  <span class="template-arrow-menu"></span>
                </a>
              </li>
            {% else %}
              <li>
                <a href="{{servei.url}}" title="{{servei.name}}">
                  {{servei.name}}
                  <span class="template-arrow-menu"></span>
                </a>
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      </div>
      <div class="column column-3-4">
        <div class="row">
          <div class="column column-1-2">
            <a href="{{page.image}}" class="prettyPhoto re-preload" title="{{page.title}}">
              <img src="{{page.image}}" alt="img" style="display: block;">
            </a>
          </div>
          <div class="column column-1-2">
            <a href="{{page.image2}}" class="prettyPhoto re-preload" title="{{page.title}}">
              <img src="{{page.image2}}" alt="img" style="display: block;">
            </a>
          </div>
        </div>
        {% if content %}
        <div class="row page-margin-top">
          <div class="column-1-1">
            <h3 class="box-header">DESCRIPCIÓ DEL SERVEI</h3>
            <p class="description t1">{{content}}</p>
          </div>
        </div>
        {% endif %}
        <div class="row page-margin-top padding-bottom-70">
          {% include why_us.html %}
          {% include faq.html %}
        </div>
      </div>
    </div>
  </div>
</div>

