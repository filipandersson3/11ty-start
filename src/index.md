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