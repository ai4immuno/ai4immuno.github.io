---
layout: page
title: News
nav_exclude: true
description: A feed containing all of the project news.
---

# Announcements

Announcements are stored in the `_announcements` directory and rendered according to the layout file, `_layouts/announcement.html`.

{% assign news = site.news | reverse %}
{% for new in news %}
{{ news }}
{% endfor %}
