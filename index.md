---
layout: page
title: 
<!-- tagline: Supporting tagline -->
---
{% include JB/setup %}
<ul class="posts ui animated list">
	{% for post in site.posts %}
	<li class="item"><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}
</ul>
<p></p>