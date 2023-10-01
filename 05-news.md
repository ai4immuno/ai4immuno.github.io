---
layout: page
title: News
nav_exclude: false
description: A feed containing all of the project news.
permalink: /news/
has_children: true
nav_order: 5
---


# Announcements

Announcements are stored in the `_announcements` directory and rendered according to the layout file, `_layouts/announcement.html`.

{% assign news = site.news | reverse %}
{% for new in news %}
{{ news }}
{% endfor %}
