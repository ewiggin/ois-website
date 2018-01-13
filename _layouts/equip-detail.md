---
title: Team layout
date: 2018-01-01 13:13:00 +01:00
layout: default
---

<div class="theme-page padding-bottom-70">
    <div class="row gray full-width page-header vertical-align-table">
      <div class="row full-width padding-top-bottom-50 vertical-align-cell">
        <div class="row">
          <div class="page-header-left">
            <h1>{{page.name}}</h1>
          </div>
          <div class="page-header-right">
            <div class="bread-crumb-container">
              <label>Estas aqui:</label>
              <ul class="bread-crumb">
                <li>
                  <a title="Our Team" href="#">
                    EQUIP
                  </a>
                </li>
                <li class="separator">
                  /
                </li>
                <li>
                  {{page.name}}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="clearfix">
      <div class="row page-margin-top-section">
        <div class="column column-1-3">
          <div class="team-box single">
            <a href="#" title="{{page.name}}">
              <img alt="{{page.name}}" src="{{page.image}}" style="display: block; width:100%;">
            </a>
            <div class="team-content">
              <h4>
                <a href="#" title="{{page.name}}">{{page.name}}</a>
                <span>FUNDADOR</span>
              </h4>
            </div>
            <ul class="social-icons" style="left: 109px; display: none; top: 247px;">
              <li><a title="" target="_blank" href="http://facebook.com/" class="social-facebook">&nbsp;</a></li>
              <li><a title="" target="_blank" href="http://twitter.com/" class="social-twitter">&nbsp;</a></li>
              <li><a title="" target="_blank" href="http://linkedin.com" class="social-linkedin">&nbsp;</a></li>
            </ul>
          </div>
        </div>
        <div class="column column-1-3">
          <h3 class="box-header">RESUM</h3>
          <table class="margin-top-40 align-left">
            <tbody>
              <tr>
                <td>Nom: {{page.name}}</td>
              </tr>
              <tr>
                <td>Adreça: Carrer Font del Capellà 24 1º 08232 Viladecavalls, Barcelona</td>
              </tr>
              <tr>
                <td>Email: <a href="mailto:obresiserveiscarmelo@gmail.com">obresiserveiscarmelo@gmail.com</a></td>
              </tr>
              <tr>
                <td>Telèfon: +34 607 240 726</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="column column-1-3">
          <h3 class="box-header">PERFIL</h3>
          <p class="description t1 margin-top-34">
            {{content}}
          </p>
        </div>
      </div>
      <div class="row top-border page-margin-top-section full-width">
        <div class="row page-margin-top-section">
          <div class="column column-1-3">
            <ul class="features-list">
              <li class="sl-small-key">
                <h4>CLAU EN MÀ</h4>
                <p>Combinem mà d'obra de qualitat, coneixements superiors i preus ajustats.</p>
              </li>
            </ul>
          </div>
          <div class="column column-1-3">
            <ul class="features-list">
              <li class="sl-small-person">
                <h4>RECURSOS</h4>
                <p>Tenim l'experiència i els recursos per realitzar el teu projecte.</p>
              </li>
            </ul>
          </div>
          <div class="column column-1-3">
            <ul class="features-list">
              <li class="sl-small-trolley">
                <h4>SUBMINISTRAMENT</h4>
                <p>Treballem amb una sèrie de passos acuradament planificats.</p>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
