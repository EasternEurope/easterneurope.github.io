---
layout: default
title: Blog archive
---


Blog archive
========================================

<ul class="posts">
	{% for post in site.posts %}
	{% assign author = site.authors[post.author] %}
	<li>
		<a class="title" href="{{ post.url }}">{{ post.title }}</a>
		<div class="meta">
			{{ post.date | date_to_string }}
			by <strong>{{ author.display_name }}</strong>
		</div>
	</li>
	{% endfor %}
</ul>
