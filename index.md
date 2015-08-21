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
	<a class="item" href="/about.html">
		About
	</a>
</div>
<p></p>
<div class="ui">
	<ul class="posts ui list">
		{% for post in site.posts %}
		<li class="">
			<h3 class=""><a href="{{ BASE_PATH }}{{ post.url }}" style="color: #159957;">{{ post.title }}</a></h3>
			<div>
				<span class="site-footer-credits">{{ post.date | date_to_string }}</span>
			</div>
			<p></p>
		</li>
		{% endfor %}
	</ul>
</div>
