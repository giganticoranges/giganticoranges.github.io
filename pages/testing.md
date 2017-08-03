---
layout: page
title:  "The Robotics Institute @ Guelph"
breadcrumb: true
permalink: /testing/index.html
header:
    image: "banner.jpg"
    background-color:  "#FFFFFF"
image:
    thumb: "banner.jpg"
---

<div class="row t30">
 <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
 <div class="medium-12 columns">
  <article itemscope itemtype="http://schema.org/Article">
  <header>
  <div itemprop="name">
  </div>
  </header>

  <div itemprop="articleSection">
  <ol>

  <div class="w3-content w3-section" style="max-width:500px">
   <img class="mySlides w3-animate-fading" src="{{site.baseurl}}/images/index-1.jpg" style="width:100%"/>
   <img class="mySlides w3-animate-fading" src="{{site.baseurl}}/images/index-2.jpg" style="width:100%"/>
   <img class="mySlides w3-animate-fading" src="{{site.baseurl}}/images/index-3.jpg" style="width:100%"/>
  </div>

  <script>
   var slideIndex = 0;
   carousel();

   function carousel() {
    var i;
    var x = document.getElementsByClassName("mySlides");
    for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
   }
   slideIndex++;
   if (slideIndex > x.length) {slideIndex = 1}
    x[slideIndex-1].style.display = "block";
    setTimeout(carousel, 5000);
   }
  </script>

<p>The Robotics Institute @ Guelph is an advanced research lab within the School of Engineering. The main research areas include robotic grasping and manipulation, human robot interaction, rehabilitation robotics, mechatronics, robot learning and robot vision.  Application areas include service robots in agriculture and health care as well as traditional applications of robotics in manufacturing, food processing, and automotive. The institute has strong record of working with industrial partners in various industries.</p>
<h2>Mission Statement</h2>

<br>The Institute’s mandate is to encourage collaboration and education in order to advance non-traditional robotics research.
