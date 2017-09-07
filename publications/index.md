---
layout: archive
title: "PUBLICATIONS"
date: 2014-05-30T11:40:45-04:00
modified:
excerpt: "Our publications."
tags: []
image:
  feature:
  teaser:
---

{% assign posts = "publication1,
					publication2, 
						publication3
						"| split: ',' %}

<div class="archive-wrap">
	<div class="page-content">
		<div class="tiles">
			{% for post in posts %}
				<article class="tile" itemscope itemtype="http://schema.org/Article">
					<h2 class="post-title" itemprop="name">{{ post }}</h2>
				</article>
			{% endfor %}
		</div><!-- /.tiles -->
	</div><!-- /.page-content -->
</div><!-- /.archive-wrap -->

