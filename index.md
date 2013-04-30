---
layout: page
title: 送别花的DNA
tagline: 快到碗里来~~~
---
{% include JB/setup %}

{% for post in site.posts limit 4 %}
## {{ post.date | date_to_string }} &raquo; [{{ post.title }}]({{ BASE_PATH }}{{ post.url }})

<div class="entry-content">
{{ post.content | truncatewords:30}}
<div>

<a href="{{ post.url }}">Read more...</a><br><br>
{% endfor %}
