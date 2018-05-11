---
layout: default
title: Categories
description: List of posts according to their categories.
keywords: Categories
---

<div class='tag_cloud'>
<ul>
{% for cat in site.categories %}
<a href="#{{ cat[0] }}" title="{{ cat[0] }}" rel="{{ cat[1].size }}">{{ cat[0] }}({{ cat[1].size }})</a>
<span style="display:inline-block; width: 1em;"></span>
{% endfor %}
</ul>
</div>

{% for category in site.categories %}
<h3>{{ category | first }}</h3>
<ul id="{{ category[0] }}">
{% for post in category.last %}
<li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a> <b> ({{ post.date | date: "%m/%d/%Y" }}) </b></li>
{% endfor %}
</ul>
{% endfor %}
