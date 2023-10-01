---
layout: page
title: Team
description: A listing of all the team members
permalink: /team/
has_children: true
nav_order: 6
---

{:toc}


# Our Team

Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Main AI4Immuno Leads

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Faculty Sponsors

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
