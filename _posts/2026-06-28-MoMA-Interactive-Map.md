---
layout: post
title: "Week 3: Using Museum Data Set to Create Interactive Interface"
date: 2026-06-14
---

This week, we experimented with museum's online collections through their data sets uploaded on github. 



![Interactive Map](/assets/images/week3/InteractiveMap.jpg)


<div class="two-grid">
  <img src="/assets/images/week3/ArtistsInUK.jpg"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/week3/listOfArtists.jpg"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/week3/AnnanWorks.jpg"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/week3/specificWork.jpg"
     onclick="openLightbox(this.src)">
</div>

<div id="lightbox" onclick="this.style.display='none'">
  <img id="lightbox-img">
</div>




<script>
function openLightbox(src) {
  document.getElementById("lightbox").style.display = "flex";
  document.getElementById("lightbox-img").src = src;
}
</script>


