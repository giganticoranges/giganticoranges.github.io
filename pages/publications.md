---
layout: page
title:  "Publications"
breadcrumb: true
permalink: /publications/index.html
header:
    image: "banner.jpg"
    background-color:  "#FFFFFF"
---

<div class="row t30">
	<div class="medium-12 columns">
		<article itemscope itemtype="http://schema.org/Article">

			<div itemprop="articleSection">
   			<ol>

			<h3>Journals (selected)</h3>

			{% for post in site.categories.journals %}
				{{ post.excerpt }}
			{% endfor %}

			<h3>Conferences (selected)</h3>

			{% for post in site.categories.conferences %}
				{{ post.excerpt }}
			{% endfor %}
