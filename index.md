---
layout: default
---

# Posts

{% for post in site.posts %}
<article class="post">
	<h2>{{ post.title }}</h2>
	{% include date.liquid date=post.date updated=post.updated %}
	{{ post.excerpt }}
	<a href="{{ post.url | relative_url}}">read more</a>
</article>
{% endfor %}