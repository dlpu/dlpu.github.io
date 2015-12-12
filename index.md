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
					<h3 class=""><a href="{{ BASE_PATH }}{{ post.url }}" style="color: #000;">{{ post.title }}</a></h3>
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
			<a href="http://weibo.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -469px -5px no-repeat;" class="sns"></a>
			<a href="https://twitter.com/tcitry" target="_blank" style="background: url('/image/sns_bg.png') -4px -5px no-repeat;" class="sns"></a>
		</div>

		<div style="margin-left: 20px;">
			我比较懒，个人搭建的博客在图片上传或是图片URL地址的处理上有点麻烦，同时我也想有一些交流，所以我尝试在简书或者SegmentFault上面发一些内容（那里图片可以直接Ctrl-V），等思路都捋顺了，最后发到博客上。
			<ul>
				<li><a href="http://www.jianshu.com/users/4ff4d2e2b16c">简书</a>主要是扯淡方面</li>
				<li><a href="http://segmentfault.com/blog/tcitry">SegmentFault</a>主要是技术方面</li>
			</ul>
		</div>
	</div>
</div>
