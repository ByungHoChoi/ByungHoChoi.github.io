---
layout: archive
title: Paper Reviews
permalink: /papers/
category: papers
author_profile: true
---

Short reviews and notes from papers I read.

{% assign archive_posts = site.categories[page.category] %}
{% for post in archive_posts %}
  {% include archive-single.html %}
{% endfor %}
