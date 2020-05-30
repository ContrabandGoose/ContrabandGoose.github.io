---
title: "Control PCB"
date: 2020-05-25
tags: [CAD, solidworks, KiCad]
header:
  image: "/project files/Harting Cable/harting cable.jpg"
excerpt: "Control PCB used in the Bench top amplifier project to drive the RF circuit and the display PCB"
mathjax: "true"
---

This was the first PCB i worked on. I started out with just a circuit diagram and a recomendation to try using KiCad, I'm glad I tried it out! I've layed out some PCB's manually using Autocad LT and it really doesn't compare to a program like KiCad. The whole process is streamlined and easy to use out of the box, lots of footprints and its easy to change or amend footprints to suit the need. This PCB and the other two PCB's I desgined for the bench top amplifier have gone through a few revisions after the first development PCB's where made.


## Model

I've provided a step model. Unfortunately I'm still looking for a simple solution to export KiCad PCB's into Solidworks, I've been plotting DXF's from KiCad then importing them into Solidworks but the traces have so many contours that usually solidworks crashes trying to extrude the profiles. For now I use a blanck PCB's with the right hole locations to provide the most accurate assembly drawing.

<html>
  <iframe scrolling='no' frameborder='0' allowfullscreen='true' src='https://www.3dcontentcentral.com/external-site-embed.aspx?format=3D&catalogid=171&modelid=1352939&width=250&height=250&edraw=true' name='PreviewFrame3D' id='PreviewFrame3D' width='800' height='600'></iframe><br/><a href='https://www.3dcontentcentral.com/download-model.aspx?catalogid=171&id=1352939'>Download</a>
  </html>


## Drawing

<embed src="{{ site.url }}{{ site.baseurl }}/project files/Bench Top Amplifier/Control PCB.PDF" type="application/pdf" width='800' height='700'>




<html>
  <!-- The grid: four columns -->
<div class="row">
  <div class="column">
    <img src="{{ site.url }}{{ site.baseurl }}/project files/Bench Top Amplifier/PCB photos/Control Board Prototype.jpg" alt="Prototype" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="{{ site.url }}{{ site.baseurl }}/project files/Bench Top Amplifier/PCB photos/Control Board 1.jpg" alt="Production version front" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="{{ site.url }}{{ site.baseurl }}/project files/Bench Top Amplifier/PCB photos/Control Board 2.jpg" alt="Production version front" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="{{ site.url }}{{ site.baseurl }}/project files/Bench Top Amplifier/PCB photos/Control Board 3.jpg" alt="Production version rear" onclick="myFunction(this);">
  </div>
</div>

<!-- The expanding image container -->
<div class="container">
  <!-- Close the image -->
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>

  <!-- Expanded image -->
  <img id="expandedImg" style="width:100%">

  <!-- Image text -->
  <div id="imgtext"></div>
</div>
<style>
  /* The grid: Four equal columns that floats next to each other */
.column {
  float: left;
  width: 25%;
  padding: 10px;
}

/* Style the images inside the grid */
.column img {
  opacity: 0.8;
  cursor: pointer;
}

.column img:hover {
  opacity: 1;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* The expanding image container (positioning is needed to position the close button and the text) */
.container {
  position: relative;
  display: none;
}

/* Expanding image text */
#imgtext {
  position: absolute;
  bottom: 15px;
  left: 15px;
  color: white;
  font-size: 20px;
}

/* Closable button inside the image */
.closebtn {
  position: absolute;
  top: 10px;
  right: 15px;
  color: white;
  font-size: 35px;
  cursor: pointer;
}
</style>
<script>
  function myFunction(imgs) {
  // Get the expanded image
  var expandImg = document.getElementById("expandedImg");
  // Get the image text
  var imgText = document.getElementById("imgtext");
  // Use the same src in the expanded image as the image being clicked on from the grid
  expandImg.src = imgs.src;
  // Use the value of the alt attribute of the clickable image as text inside the expanded image
  imgText.innerHTML = imgs.alt;
  // Show the container element (hidden with CSS)
  expandImg.parentElement.style.display = "block";
}
</script>
</html>
