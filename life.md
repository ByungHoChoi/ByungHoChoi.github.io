---
layout: archive
title: Daily Life
permalink: /life/
category: life
author_profile: true
---

Small records from ordinary days.

{% assign archive_posts = site.categories[page.category] %}
{% for post in archive_posts %}
  {% include archive-single.html %}
{% endfor %}
