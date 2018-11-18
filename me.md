---
layout: page
title: About me
permalink: /about-me/
---

My name is Fredrik Sundberg. I was born and raised in Lund, Sweden, however I am currently studying web programming at Linneaus University in Kalmar, developing my development skills!

## Interests
Some of my interests include:

<ul>
  {% for track in site.data.about.interests %}
    <li>{{ track }}</li>
  {% endfor %}
</ul>
