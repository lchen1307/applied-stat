---
layout: page
title: Textbook
nav_exclude: true
description: A feed containing all of the class announcements.
---

# Textbook

Announcements are stored in the `_announcements` directory and rendered according to the layout file, `_layouts/announcement.html`.

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
