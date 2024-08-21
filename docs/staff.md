---
layout: page
title: Staff
permalink: /staff/
nav_order: 2
---

# Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

# Teaching Assistants

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

# Course Assistants

{% assign course_assistants = site.staffers | where: 'role', 'Course Assistant' %}
{% assign num_course_assistants = course_assistants | size %}
{% if num_course_assistants != 0 %}

{% for staffer in course_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}