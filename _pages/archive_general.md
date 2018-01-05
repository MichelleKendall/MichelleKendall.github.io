---		
 layout: archive		
 title: General	
 permalink: /general/
---		

<div class="tiles">
{% for post in site.categories.general %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->