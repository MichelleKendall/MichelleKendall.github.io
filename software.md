---
layout: archive
title: Software
permalink: /software/
image:
  feature: knitted_tree_banner.jpg
---

I maintain the R packages <a href="https://cran.r-project.org/web/packages/treespace/index.html" target="_blank">*treespace*</a> 
and <a href="https://cran.r-project.org/web/packages/phyloTop/index.html" target="_blank">*phyloTop*</a>.
The posts below give some more detail about each of the projects, and how to get started using them.

I also contribute to various other R packages - see <a href="https://github.com/MichelleKendall" target="_blank">my GitHub page</a> for the latest projects.

<div class="tiles">
{% for post in site.categories.software %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->