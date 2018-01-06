---
layout: archive
permalink: /general
title: "General Posts"
image:
  feature: knitted_tree_banner.jpg
---

<div class="tiles">
{% for post in site.categories.general %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->