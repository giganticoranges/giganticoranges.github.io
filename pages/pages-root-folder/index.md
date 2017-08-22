---
layout: page
permalink: /index.html
breadcrumb: true
header:
    image: banner.jpg
    background-color:  "#FFFFFF"
image:
    thumb: "banner.jpg"
Home: true
---

<style>
* {box-sizing:border-box}
.mySlides {display:none}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  border: 0;
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 0 0 0;
}

/* Position the "next button" to the right */
.next {
  border: 0;
  right: 0;
  border-radius: 0 0 0 0;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  border: 0;
  background-color: rgba(0,0,0,0.8);
}

/* The dots/bullets/indicators */
.dot {
  border: 0;
  cursor:pointer;
  height: 13px;
  width: 13px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  border: 0;
  border-radius: 25px;
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
</style>
<body>

<div class="slideshow-container">

<div class="mySlides fade">
  <img src="{{site.baseurl}}/images/index-1.jpg" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="{{site.baseurl}}/images/index-2.jpg" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="{{site.baseurl}}/images/index-3.jpg" style="width:100%">
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
}
</script>

  <h1><br>The Robotics Institute @ Guelph</h1>

  <p>The Robotics Institute @ Guelph is an advanced research lab within the School of Engineering. The main research areas include robotic grasping and manipulation, human robot interaction, rehabilitation robotics, mechatronics, robot learning and robot vision.  Application areas include service robots in agriculture and health care as well as traditional applications of robotics in manufacturing, food processing, and automotive. The institute has strong record of working with industrial partners in various industries.</p>
