---
layout: page
title: 殷东亮的博客
<!-- tagline: Supporting tagline -->
---
{% include JB/setup %}
<div style="margin-bottom: 20px;">
<a href="/" class="">Home</a> | <a href="/archive.html" class="">Archive</a> | <a href="/tags.html" class="">Tags</a> | <a href="/about.html" class="">About</a>
</div>
<ul class="posts ui animated list">
	{% for post in site.posts %}
	<li class="item"><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
	{% endfor %}
</ul>
<p></p>