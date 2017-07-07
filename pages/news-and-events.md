---
layout: page
title:  "News and Events"
breadcrumb: true
permalink: /news-and-events/index.html
header:
    image: "banner.jpg"
    background-color:  "#FFFFFF"
---


{% for post in site.categories.news %}
<div class="row">
	<div class="small-12 columns">
 	
		<sub>{{ post.date | date: '%B %d, %Y' }}</sub>
		<h3>{{ post.title }}</h3>

	  	{{ post.excerpt }}

	</div>
</div>
{% endfor %}
