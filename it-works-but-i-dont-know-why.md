---
layout: series
title: It Works But I Don't Know Why
description: In this series, we are exploring ecouraging insights and techniques to mentally deal with the sentiment of not understanding how to use a system or framework in your everyday work.
comments: true
published: true
---

## It Works But I Don't Know Why
<br/>
<img src="img/action-plan-brainstorming-complex-212286.jpg" width="342" height="228">

*In this series, we are exploring ecouraging insights and techniques to <br/> mentally deal with the sentiment of not understanding <br/> how to use a system or framework in your everyday work.*

{% if site.categories.it-works-but-i-dont-know-why %}
   {% assign posts = site.categories.it-works-but-i-dont-know-why | sort: "series-part" %}
   {% for post in posts %}
      <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }} {{ post.sub-title }}</a>
   {% endfor %}
{% endif %}