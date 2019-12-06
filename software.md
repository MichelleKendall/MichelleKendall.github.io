---
layout: archive
title: Software
permalink: /software/
---

I maintain the R packages <a href="https://cran.r-project.org/web/packages/treespace/index.html" target="_blank">*treespace*</a>
and <a href="https://michellekendall.github.io/phyloTop/" target="_blank">*phyloTop*</a>.
The links below give some more detail about each of these projects and how to get started using them.

I also contribute to various other R packages - see <a href="https://github.com/MichelleKendall" target="_blank">my GitHub page</a> for the latest projects.

<div class="tiles">
{% for post in site.categories.software %}
  {% include post-grid-no-date.html %}
{% endfor %}
</div><!-- /.tiles -->
