---
layout: page
title: Projects
permalink: /projects/
---

These are various personal projects and school assignments that I've done (or am working on).

<!--
projects are sorted by most recent.
special thanks to the creator of this gist: https://gist.github.com/Phlow/1f27dfafdf2bbcc5c48e for showing how to reverse the date order.
-->
{% assign sorted = site.projects | sort: 'date' |reverse %}
{% for project in sorted %}
- [{{ project.title }}]({{project.url}}): {{ project.description }}
{% endfor %}