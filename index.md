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
			<a href="http://segmentfault.com/u/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -520px -5px no-repeat;" class="sns"></a>
			<a href="http://www.zhihu.com/people/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -314px -5px no-repeat;" class="sns"></a>
			<a href="http://www.douban.com/people/yindongliang/" target="_blank" class="sns">
				<img src="/image/douban.png" class="sns-img"></a>
			<a href="https://twitter.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -4px -5px no-repeat;" class="sns"></a>
		</div>

		<div style="margin-left: 20px;">
			<div>关于作者</div>
			<div>
				<iframe width="100%" height="550" class="share_self"  frameborder="0" scrolling="no" src="http://widget.weibo.com/weiboshow/index.php?language=&width=0&height=550&fansRow=2&ptype=1&speed=0&skin=1&isTitle=1&noborder=1&isWeibo=1&isFans=0&uid=2510226067&verifier=ef835547&dpc=1"></iframe>
			</div>
			<div>
				<a class="twitter-timeline" href="https://twitter.com/tcitry" data-widget-id="455901943076896768">@tcitry的推文</a>
				<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>
			</div>
		</div>
	</div>
</div>
