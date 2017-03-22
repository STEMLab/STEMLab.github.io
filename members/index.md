---
layout: archive
title: ""
date: 2014-05-30T11:39:03-04:00
modified:
excerpt: "Spatio-Temporal Databases Laboratory Members."
tags: []
image: 
  feature:
  teaser: 
---

<div class="tiles">
{% for post in site.categories.members %}
	<div class="tile">
		<table>
			<tr>
				{% if post.image.teaser %}
				<td>
					<a href="{{ site.url }}{{ post.url }}">
					<img src="{{ site.url }}/images/{{ post.image.teaser }}" alt="teaser" itemprop="image">
					</a>
				</td>
				{% else %}
				<td>
					<a href="{{ site.url }}{{ post.url }}">
						<img src="{{ site.url }}/images/{{ site.teaser }}" alt="teaser" itemprop="image">
					</a>
				</td>
				{% endif %}
				<td>{% include post-grid.html %}</td>
			</tr>
		</table>
	</div>
{% endfor %}
</div><!-- /.tiles -->