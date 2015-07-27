---
layout: page
title: 殷东亮的博客
<!-- tagline: Supporting tagline -->
---
{% include JB/setup %}

<div class="ui secondary pointing menu">
	<a class="active item" href="/">
		Home
	</a>
	<a class="item" href="/archive.html">
		Archive
	</a>
	<a class="item" href="/tags.html">
		Tags
	</a>
	<a class="ui item" href="/about.html">
		About
	</a>
</div>
<div class="ui segment">
	<ul class="posts ui animated list">
	{% for post in site.posts %}
	<li class="item"><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}
</ul>
</div>
