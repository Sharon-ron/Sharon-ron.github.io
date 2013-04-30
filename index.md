---
layout: page
title: 送别花的DNA
tagline: 快到碗里来~~~
---
{% include JB/setup %}

{% for post in site.posts limit 4 %}
## {{ post.date | date_to_string }} &raquo; [{{ post.title }}]({{ BASE_PATH }}{{ post.url }})

<div class="entry-content">
{{ post.content | strip_html | truncatewords:30}}
</div>

<a href="{{ post.url }}">Read more...</a><br><br>

---
{% endfor %}
<p>
    <a class="btn btn-primary btn-large" href="{{ BASE_PATH }}{{ site.JB.archive_path }}">
	All Posts
    </a>
</p>
