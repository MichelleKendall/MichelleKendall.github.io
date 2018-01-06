---
layout: archive
permalink: /archives/general
title: "General Posts"
image:
  feature: feature_image_demo.png
---

<div class="tiles">
{% for post in site.categories.general %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->