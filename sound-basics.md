---
layout: series
title: Sound Basics
description: A series of writings providing a gentle introduction into the physics of sound and how it is represented and manipulated in the digital realm.
comments: true
---

## Sound Basics
<br/>
<img src="img/sound-wave.svg" width="150" height="130">
*An ongoing series of writings providing a gentle introduction into the physics of sound <br/> and how it is represented and manipulated in the digital realm.*

{% assign posts = site.categories.sound-basics | sort %}
{% for post in posts %}
  <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
{% endfor %}