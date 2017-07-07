---
layout: page
title:  "Research Projects"
breadcrumb: true
permalink: /research-projects/index.html
header:
    image: "banner.jpg"
    background-color:  "#FFFFFF"
---

<div class="row t30">
 {% for post in site.categories.research-projects %}
  {% capture modulo %}{{ forloop.index | divided_by: 4.0 }}{% endcapture %}

  {% if forloop.index == site.categories.research-projects.size %}
   {% capture lastModulo %}{{ forloop.index | divided_by: 4.0 }}{% endcapture %}
   {% if lastModulo contains '.25' %}
    <div class="small-12 columns">
   {% endif %}
   {% if lastModulo contains '.5' %}
    <div class="small-9 columns">
   {% endif %}
   {% if lastModulo contains '.75' %}
    <div class="small-6 columns">
   {% endif %}
   {% if lastModulo contains '.0' %}
    <div class="small-3 columns">
   {% endif %}
  {% else %} 
   <div class="small-3 columns">
  {% endif %}

   <a href="{{site.baseurl}}{{ post.permalink }}"><img src="{{site.baseurl}}/images/{{ post.preview }}" /></a>

  </div>

  {% if modulo contains '.0' %}
   </div>
   <div class="row t30">
  {% endif %}

 {% endfor %}
</div>

