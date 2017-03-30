---
layout: group
title: Activity-Modeling Platforms
category: abm-platform
front: true
---

The following is a list of the projects 


<section class="tiles">

{% for group in site.project-groups %}
  	{% if group.tags contains page.category %}
  		<article class="style1 bigtile">
  			{% if project.img %}
  			<img src='{{ site.url }}/img/{{ group.img }}' alt="" />
  			{% else %}
  			<img src='{{ site.url }}/img/{{ site.default-tile-img }}' alt="" />
  			{% endif %}
    		<a href='{{ group.url }}'>
				<h2>{{ group.title }}</h2>
				<div class="content">
					<p>{{ group.short-description }}</p>
				</div>
			</a>
  		</article>
  
  	{% endif %}
{% endfor %}

															
{% for project in site.projects %}
  	{% if project.tags contains page.category %}
  		<article class="style1 bigtile">
  			{% if project.img %}
  			<img src='{{ site.url }}/img/{{ project.img }}' alt="" />
  			{% else %}
  			<img src='{{ site.url }}/img/{{ site.default-tile-img }}' alt="" />
  			{% endif %}
    		<a href='{{ project.url }}'>
				<h2>{{ project.title }}</h2>
				<div class="content">
					<p>{{ project.short-description }}</p>
				</div>
			</a>
  		</article>
  
  	{% endif %}
{% endfor %}

</section>






