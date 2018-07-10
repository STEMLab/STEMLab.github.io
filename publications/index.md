---
layout: publication
title: "PUBLICATIONS"
date: 2014-05-30T11:40:45-04:00
modified:
excerpt: "Our publications."
tags: []
image:
  feature:
  teaser:
---
<div class="archive-wrap">
	<div class="page-content">
		<div class="tiles">
			{% for post in site.categories.publications %}
        {% assign items = post.content | newline_to_br | split: '<br />' %}
        {% for item in items %}
  				<article itemtype="http://schema.org/Article">
  					<h2 class="post-title" itemprop="name">{{ item }}</h2>
  				</article>
        {% endfor %}
			{% endfor %}
		</div><!-- /.tiles -->
	</div><!-- /.page-content -->
</div><!-- /.archive-wrap -->
