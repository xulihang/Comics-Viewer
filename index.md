---
layout: default
---
<h1>多模态语言学习</h1>
<ul class="post-list">
	{% for post in site.posts reversed %}
	<li>
		<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">[{{post.series}}]{{ post.title }}</a> <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
	</li>
	{% endfor %}
</ul>