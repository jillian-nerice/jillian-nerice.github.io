---
layout: post
title: "Week 3: Using Museum Data Set to Create Interactive Interface"
date: 2026-06-14
---


This week, we experimented with museum's online collections through their data sets uploaded on github. We learned that many museums nowadays have open access API's available to increase the accessibility of their collections. Using the data available online, I created an interactive map as a way to explore the collection of the Museum of Modern Art geographically.

![Interactive Map](/assets/images/week3/InteractiveMap.jpg)

The interactive map I created allows the users to visually see the distribution of the artists in the MoMA collection by their country of origin. The countries are colour coded by the number of artists from that area featured in the MoMA collection, with the darker colours indicating more artists and lighter colours indicating less artists. Hovering over the country allows the user to see the exact number of artists from that region within MoMA. The sidebar offers more information on the artists, as some artists in the collection come from the same land geographically but identify differently. For example, within the United States of America, there are Native American artists, Oneida, Tlingit, etc. When creating the map, I grouped artists together geographically, but I also preserved the nuanced identities as they appeared in the data set. 

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


Clicking on either the country on the map or the name of the country in the side bar navigates the user to a page of the subgroups within a country if they exist, or directly to a page where the user can look through the artists of a country. Clicking on the United Kingdom takes the user to a page where they can choose British, Welsh, Scottish, or English artists. In the artists page, the user can filter by gender or sort alphabetically, or timewise by the artists' years of birth. Clicking on a specific artist takes the user to a page of their works. The art can be seen through images that expand when clicked, or a link to the MoMA website. 

In addition to the interactive map, I also created a timeline that allows users to choose a decade and view all artists born in that decade. 

![Interactive Map](/assets/images/week3/timeline.jpg)

While creating this explorer for the MoMA, I was able to learn a lot about the initiatives museums have been taking to incorporate digital technology to reach more people. For example, the Cleveland Museum of Art incorporated a screen in their museums, where users can take a photo and have their face matched to an artwork in the museum. An email would be sent to the user with the artwork and information about it. 

This is similar to an exhibition we saw on a visit to LifeHub at Msheireb, where visitors could take a photo and have it regenerated in the style of a chosen artist. 

<div class="two-grid">
  <img src="/assets/images/week3/msheirebDali.jpg"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/week3/msheirebPicasso.jpg"
     onclick="openLightbox(this.src)">
</div>
These images are meant to be in the style of Dali and Picasso. 

These ways of engaging a visitor are similar in the sense that it involves the user of the technology to allow give an immersive experience. However, the MoMA uses AI to connect visitors to human artists by finding similarities in the viewers' images to existing works, while the LifeHub installation generated a new image inspired by an artist. 

Another way LifeHub implemented technology to engage their visitors was through an interactive screen where users could choose different food groups (dairy, meat, vegetables, nuts, etc), and categorise them by how frequently they consume them. Afterwards, it calculates an approximate carbon footprint based on the choices. 

![FoodChoice](/assets/images/week3/foodChoice.jpg)

I found this section to be quite effective in delivering an educational experience because it cognitively engages the viewer and makes them think about their choices, where the generated image activity was quite passive. 

Overall, this week I was able to learn more about the different ways technology is used to increase the ways museums are able to reach their audiences and deliver different types of experiences. I found it interesting creating my own interactive map to implement a way for people to view and access the collection of the Museum of Modern Art. I think a similar navigation system would be possible to implement at mathaf. However, there are some challenges that still need to be addressed. 

For example, some artists in the database had unknown origins, and so they are not included in the explorer I created. Furthermore, it might be difficult to preserve more nuanced identities with a navigator like this, as it defines an artist by their birth place or nationality. This makes it difficult to navigate artists who have complex identities, such as mixed artists or artists who frequently move places. 



<script>
function openLightbox(src) {
  document.getElementById("lightbox").style.display = "flex";
  document.getElementById("lightbox-img").src = src;
}
</script>


