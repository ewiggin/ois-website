---
name: Projects detail layout
layout: default
---
<div class="theme-page padding-bottom-66">
  <div class="row gray full-width page-header vertical-align-table">
    <div class="row full-width padding-top-bottom-50 vertical-align-cell">
      <div class="row">
        <div class="page-header-left">
          <h1>{{page.title}}</h1>
        </div>
      </div>
    </div>
  </div>
  <div class="clearfix">
    <div class="row margin-top-70">
      <div class="column column-1-2">
        {% if page.image1 %}
          <a href="{{page.image1}}" class="prettyPhoto re-preload" title="{{page.title}}">
            <img src="{{page.image1}}" alt="img" style="display: block; width:100%;">
          </a>
        {% endif %}
        {% if page.image2 and page.image3 %}
          <div class="row margin-top-30">
            <div class="column column-1-2">
              <a href="{{page.image2}}" class="prettyPhoto re-preload" title="{{page.title}}">
                <img src="{{page.image2}}" alt="img" style="display: block; width:100%;">
              </a>
            </div>
            <div class="column column-1-2">
              <a href="{{page.image3}}" class="prettyPhoto re-preload" title="{{page.title}}">
                <img src="{{page.image3}}" alt="img" style="display: block; width:100%;">
              </a>
            </div>
          </div>
        {% endif %}
        {% if page.image4 %}
          <div class="row margin-top-30">
            <a href="{{page.image4}}" class="prettyPhoto re-preload" title="{{page.title}}">
              <img src="{{page.image4}}" alt="img" style="display: block; width:100%;">
            </a>
          </div>
        {% endif %}
      </div>
      <div class="column column-1-2">
        <h3 class="box-header">BREU DESCRIPCIÓ</h3>
        <div class="description t1">
          {{content}}
        </div>
        <h4 class="box-header page-margin-top">D'UNA ULLADA</h4>
        <table class="margin-top-40">
          <tbody>
            {% if page.type %}
            <tr>
              <td>Tipus de projecte</td>
              <td>{{page.type}}</td>
            </tr>
            {% endif %}
            {% if page.client %}
            <tr>
              <td>Client</td>
              <td>{{page.client}}</td>
            </tr>
            {% endif %}
            {% if page.finish_at %}
            <tr>
              <td>Data de finalització</td>
              <td>{{page.finish_at}}</td>
            </tr>
            {% endif %}
            {% if page.size %}
            <tr>
              <td>Mida del projecte</td>
              <td>{{page.size}}</td>
            </tr>
            {% endif %}
            {% if page.price %}
            <tr>
              <td>Valor del contracte</td>
              <td>{{page.price}}</td>
            </tr>
            {% endif %}
          </tbody>
        </table>
      </div>
    </div>
  </div>
</div>
