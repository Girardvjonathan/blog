---
layout: single
title: My achievements
date: '2021-12-31T19:33:59.191Z'
category: reflections
tags:
  - reflections
  - achievements
summary: Summary of the article
---
<link rel="stylesheet" href="/assets/css/timeline.css">
<div class="timeline">
{% for achievement in site.data.achievements %}
  <div class="container {% cycle 'left', 'right' %}">
    <div class="date">{{achievement.date}}</div>
    <i class="icon fa fa-home"></i>
    <div class="content">
      <h2>{{achievement.title}}</h2>
      {% if achievement.description %}
        <p>
          {{achievement.description}}
        </p>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>