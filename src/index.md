---
title: "Title"
layout: "base.njk"
templateEngineOverride: njk,md
---

test test

## From the Blog

{% for post in collections.posts | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}

## Articles
<ul>
{% for article in collections.articles %}
<li><a href="{{ article.url }}">{{ article.data.title }}</a></li>
{% endfor %}
</ul>