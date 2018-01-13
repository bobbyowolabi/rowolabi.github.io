---
layout: page
title: Sound Basics
description: foo
---

## Sound Basics
<img src="img/sound-wave.svg" width="150" height="130">
{{ page.description }}

{% assign posts = site.categories.sound-basics | sort %}
{% for post in posts %}
  <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
{% endfor %}