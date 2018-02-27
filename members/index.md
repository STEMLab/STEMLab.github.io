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
{% assign members = site.categories.members | group_by: "position" %}
{% for position in site.members-order %}
	{% assign currentPosition = members | where : 'name', position | first%}
	{% for post in currentPosition.items %}
		<div class="tile">
		<table>
				{% if post.image.teaser %}
				<tr>
				<td align="center">
					<a href="{{ site.baseurl }}{{ post.url }}">
					<div style="height: 130px; width: 200px; overflow: hidden;"><img src="{{ site.baseurl }}/images/{{ post.image.teaser }}" alt="teaser" itemprop="image"></div>
					</a>
				</td>
				</tr>
				{% else %}
				<tr>
				<td align="center">
					<a href="{{ site.baseurl }}{{ post.url }}">
						<div style="height: 130px; width: 200px; overflow: hidden;"><img src="{{ site.baseurl }}/images/{{ site.teaser }}" alt="teaser" itemprop="image"></div>
					</a>
				</td>
				</tr>
				{% endif %}
				<tr><td align="center">{% include post-grid.html %}</td></tr>
		</table>
	</div>
		
	{% endfor %}
	
		
{% endfor %}
</div><!-- /.tiles -->


<div class="tiles">
</br> </br> <h3> Graduated Student </h3>
{% assign grad = site.categories.graduated %}
{% for post in grad %}
<div class="tile">
		<table>
				{% if post.image.teaser %}
				<tr>
				<td align="center">
					<a href="{{ site.baseurl }}{{ post.url }}">
					<div style="height: 130px; width: 200px; overflow: hidden;"><img src="{{ site.baseurl }}/images/{{ post.image.teaser }}" alt="teaser" itemprop="image"></div>
					</a>
				</td>
				</tr>
				{% else %}
				<tr>
				<td align="center">
					<a href="{{ site.baseurl }}{{ post.url }}">
						<div style="height: 130px; width: 200px; overflow: hidden;"><img src="{{ site.baseurl }}/images/{{ site.teaser }}" alt="teaser" itemprop="image"></div>
					</a>
				</td>
				</tr>
				{% endif %}
				<tr><td align="center">{% include post-grid.html %}</td></tr>
		</table>
	</div>
{% endfor %}


</div><!-- /.tiles -->
