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

<div class="tiles">
{% for post in site.categories.project %}
  {% include post-grid-project.html %}
{% endfor %}
</div><!-- /.tiles -->