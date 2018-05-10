---
layout: default
title: Tags
description: List of posts according to their tags.
keywords: Tags
---

<div class='tag_cloud'>
{% for tag in site.tags %}
<a href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="{{ tag[1].size }}">{{ tag[0] }}({{ tag[1].size }}) </a>
{% endfor %}
</div>

{% for tag in site.tags %}
<h3>{{ tag | first }}</h3>
<ul id="{{ tag[0] }}">
{% for post in tag.last %}
<li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
{% endfor %}
