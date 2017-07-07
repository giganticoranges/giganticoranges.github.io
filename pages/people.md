---
layout: page
title:  "People"
breadcrumb: true
permalink: /people/index.html
header:
    image: "banner.jpg"
    background-color:  "#FFFFFF"
---

<p><br></p>
<h3>Faculty and Researchers</h3>

<div class="row t30">
{% for post in site.categories.researchers %}

  	{{ post.excerpt }}

{% endfor %}
</div>


<h3>Graduate Students</h3>

<div class="row t30">
{% for post in site.categories.students %}

  	{{ post.excerpt }}

{% endfor %}
</div>


<h3>Co-op Students</h3>

<div class="row t30">
{% for post in site.categories.coop %}

  	{{ post.excerpt }}

{% endfor %}
</div>


<h3>Former Members</h3>

<p>
{% for post in site.categories.former %}

  	{{ post.teaser }}<br>

{% endfor %}
</p>


