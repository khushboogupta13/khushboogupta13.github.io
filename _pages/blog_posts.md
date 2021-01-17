---
layout: archive
title: "Blog Posts"
permalink: /blog_posts/
author_profile: true
---

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
