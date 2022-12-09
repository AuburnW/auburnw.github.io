---
layout: default
title: "Auburn W."
---

{% for post in site.posts %}
<article class="post">
	<h2>{{ post.title }}</h2>
	<div class="date">{{ post.date | date: "%B %-d, %Y" }}</div>
	{{ post.excerpt }}
	<a href="{{ post.url | relative_url}}">read more</a>
</article>
{% endfor %}