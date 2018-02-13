---
layout: archive
permalink: /blog
title: "Blog Posts"
image:
  feature: knitted_tree_banner.jpg
---

<div class="tiles">
{% for post in site.categories.general %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

<a class="twitter-timeline" data-width="400" data-height="300" data-theme="light" data-link-color="#2B7BB9" href="https://twitter.com/mishkendall?ref_src=twsrc%5Etfw">Tweets by mishkendall</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>          
