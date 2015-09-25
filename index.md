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

</div>
<div class="ui two column stackable grid container">
	<div class="column">
		<div class="ui">
			<h2></h2>
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
	</div>
	<div class="column">
		<div class="" >
			<img src="/image/wechat.png" height="200">
			<br>
		</div>
		<div style="text-align: center;">
			<a href="https://github.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -263px -5px no-repeat;" class="sns"></a>
			<a href="https://twitter.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -4px -5px no-repeat;" class="sns"></a>
			<a href="http://segmentfault.com/u/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -520px -5px no-repeat;" class="sns"></a>
			<a href="http://www.zhihu.com/people/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -314px -5px no-repeat;" class="sns"></a>
			<a href="http://weibo.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -469px -5px no-repeat;" class="sns"></a>
			<a href="http://www.douban.com/people/yindongliang/" target="_blank" class="sns">
				<img src="/image/douban.png" class="sns-img">
			</a>
		</div>
		<div>关于作者</div>


		
	</div>
</div>
