---
layout: single
title: My achievements
date: '2021-12-31T19:33:59.191Z'
category: reflections
tags:
  - reflections
  - achievements
excerpt: "This is my timeline of accomplishment through my life \U0001F604"
summary: What I accomplished through my life so far
preview: /assets/images/carolyn-christine-D7bmnvGJA2Q-unsplash.jpg
---
<link rel="stylesheet" href="/assets/css/timeline.css">
<div class="timeline">
{% for achievement in site.data.achievements %}
  <div class="container {% cycle 'left', 'right' %}">
    <div class="date">{{achievement.date}}</div>
    <!-- <i class="icon fa fa-home"></i>  TODO -->
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
