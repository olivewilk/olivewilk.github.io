---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
## Working Papers
{% assign working = site.publications | where: "publication", "Working Paper" %}
{% for post in working %}
  {% include archive-single.html %}
{% endfor %}

## Published & Forthcoming
{% assign published = site.publications | where_exp: "post", "post.publication != 'Working Paper'" %}
{% for post in published %}
  {% include archive-single.html %}
{% endfor %}
