---
layout: group
title: Full Travel Model Systems
tag: full-model-system
category: visualization
---

The following is a list of the projects 


<section class="tiles">
																
{% for project in site.projects %}
  	{% if project.tags contains page.tag %}
  	<article class="style1 bigtile">
  	<img src='{{ site.url }}/img/{{ project.img }}' alt="" />
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







