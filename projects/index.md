---
layout: archive
title: "PROJECTS"
date: 2014-05-30T11:40:45-04:00
modified:
excerpt: "Accomplished and in progress."
tags: []
image:
  feature:
  teaser:
---

<div class="archive-wrap">
      <article class="tile"><h2>In progress</h2></article>
</div><!-- /.archive-wrap -->

<div class="archive-wrap">
  <div class="page-content">
  <div class="tiles">
  {% for post in site.categories.project %}
    {% include post-grid-project.html %}
  {% endfor %}
  </div><!-- /.tiles -->
  </div><!-- /.page-content -->
</div><!-- /.archive-wrap -->

<div class="archive-wrap">
      <article class="tile"><h2>Accomplished</h2></article>
</div><!-- /.archive-wrap -->

<div class="archive-wrap">
  <div class="page-content">
  <div class="tiles">
  {% for post in site.categories.project_old %}
    {% include post-grid-project.html %}
  {% endfor %}
  </div><!-- /.tiles -->
  </div><!-- /.page-content -->
</div><!-- /.archive-wrap -->
