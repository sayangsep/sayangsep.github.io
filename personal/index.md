---
layout: page
tags: [research, sayan, ghosal, Jhu, graduate]
modified: 2020-01-08T20:53:07.573882-04:00
comments: false
---
### A Little More

---

<p style="font-family:'Arial'"> I'm grew up in a small town, Santiniketan, India. Santiniketan was lovingly modelled by Rabindranath Tagore on the principles of humanism, internationalism and a sustainable environment. I consider myself fortunate to grow up in a place that embodies Rabindranath Tagore's vision of idealism that is unfettered by religious and regional barriers. We take pride in our heritage, and we even have our own song :D

<html>
<head>
<style>
blockquote {
  margin-left: 20px;
  border-left: 3px solid #eee;
}
</style>
</head>
<body>
<blockquote>
She is our own, the darling of our hearts, Santiniketan.<br>
In the shadows of her trees we meet<br>
in the freedom of her open sky.<br>
Our dreams are rocked in her arms.<br>
Her face is a fresh wonder of love every time we see her,<br>
for she is our own, the darling of our hearts. –  Rabindranath Tagore
</blockquote>
</body>
</html>
<br>
<html>

<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: center;
  margin: auto;
}

/* Caption text */
.text {
  color: #111;
  font-size: 15px;
  padding: 8px 12px;
  position: bottom;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  height: 0px;
  width: 0px;
  margin: 0 0px;
  background-color: #bbb;
  border-radius: 0%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active {
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1s;
  animation-name: fade;
  animation-duration: 1s;
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
  .text {font-size: 11px}
}
</style>
</head>
</html>

<table>
    <col width="75%">
    <col width="40%">
    <tr>
        <td valign="center"><p style="font-family:'Arial'">I am a sports enthusiat. In the evening you will probably find me<br> outside in the gym, or in the ground. I am also a frequent<br> member and Vice President of <a href="http://www.hopkinstkd.com/home/">Hopkins Taekwondo Club</a>.</td>
        <td>
<html>
<body>

<div class="slideshow-container" id="slideshow1">

  <div class="mySlides one">
    <img src="/images/snd.jpg" style="width:100%">
	<div class="text"><em>San Diego, 2019</em></div>

  </div>
  <div class="mySlides one">
    <img src="/images/sky.jpg" style="width:100%">
	<div class="text"><em>Canada, 2016</em></div>
  </div>
  <div class="mySlides one">
    <img src="/images/ice2.jpg" style="width:100%">
<div class="text"><em>Iceland, 2020</em></div>
  </div>
  <div style="text-align:center">
    <span class="dot"></span> 
    <span class="dot"></span> 
    <span class="dot"></span> 
  </div>
</div>
</body>
</html> 
</td>
</tr>
</table>

<table>
    <col width="75%">
    <col width="40%">
    <tr>
        <td valign="center"><p style="font-family:'Arial'"> I love to travel whenever I find some time.</td>
        <td><html>
<body>
<div class="slideshow-container" id="slideshow2">

  <div class="mySlides two">
    <img src="/images/yosemite_v2.jpg" style="width:100%">
<div class="text"><em>Yosemite, 2019</em></div>
  </div>

  <div class="mySlides twos">
    <img src="/images/ice.jpg" style="width:100%">
<div class="text"><em>Iceland, 2019</em></div>
  </div>

  <div class="mySlides two">
    <img src="/images/death_valley_v2.jpg" style="width:100%">
<div class="text"><em>Death Valley, 2019</em></div>
  </div>

  <div style="text-align:center">
    <span class="dot"></span> 
    <span class="dot"></span> 
    <span class="dot"></span> 
  </div>
</div>
</body>
</html> 
</td>
</tr>
</table>


<script>
    use strict';
           
    function Make_a_slideshow(id){
        var slideIndex = 0,
        container = document.getElementById(id);

    function showSlides(){
        var slides = container.querySelectorAll('.mySlides');
        for (var i = 0; i < slides.length; i++){
            slides[i].style.display = "none";
                }
                slideIndex++;
             if (slideIndex > slides.length){
                        slideIndex = 1;
                    }
                    slides[slideIndex - 1].style.display = "block";
                    setTimeout(showSlides, 2000); // Change image every 2 seconds
                }
                showSlides();
            }
           
            //start slideshow 1
            Make_a_slideshow('slideshow1');
           
            //delay 1 second before starting slideshow 2
            setTimeout(function(){
                Make_a_slideshow('slideshow2');
            }, 0);
</script>


