---
layout: post
title: "Week 1"
date: 2026-06-14
---

In the first week of my internship at Mathaf, we focused on getting acquainted with the Museum and getting to know the visitors through observation and surveys. 

On the first day, we toured the collections of Mathaf and learned about its history. I learned that it began from the collections of Sheikh Hassan and served as an artistic hub where artists took residency and made up most of Mathaf's early collection. 

On the second day, we visited the National Museum of Qatar to observe the visitors and collect data on their interactions with the multimedia components of the museum. Afterwards, we were to analyse the data through programming tools. I chose to use R. Although we were not able to gather much data due to the small number of visitors on the day we visited, we were able to use a larger dataset collected in 2023. 

During our tour of the National Museum, we learned not only about the history of Qatar but also about the ways it uses technology to enhance the visitor experience and how it was brought to life. The large wall projections in the Formation of Qatar and Natural Environments exhibits were using a large number ofprojectors to create high resolution images. In addition, the museum had interactive screens scattered through the space to display timelines and ultra high resolution images of displays that allow visitors to zoom in to see the most intricate details. 

In the data exploration section, I aimed to conduct a multivariate analysis to see the effects of different types of multimedia components in the museum to a variable like how much a visitor learns or how high they rate the experiences. I also wanted to add an interaction variable such as age range to see if the age of the visitors affected how much they learned from interactive screens. 

However, I found challenges with the data that made me simplify my approach. Firstly, not all questions were answered in the survey, which meant that each column had a different amount of responses. In this bar chart, we can see the number of responses per question:

![Responses Per Question](/assets/images/responses.png)

This caused a lot of the variables to have a very low sample size leading to an unstable model. Secondly, some categories had very few observations which makes it difficult to establish a clear relationship. For example, we cannot judge the impact of interactive touch screen use on learning if the data only shows some combinations (high use, high learning) and not others (medium use, low learning). The limited data in some groups make it hard to establish a pattern. The sparseness of the data also caused me to reject the idea of exploring an interaction variable, as the data already contains very small groups and introducing an interaction variable would only cause more issues. 

In the end, I was able to pivot by simplifying the data. For example, in the likert scale questions, I grouped strongly agree and agree together into one variable and strongly disagree and disagree together in another to limit the number of groups, especially since the data was already sparse. I also grouped behaviour variables together ( never/rarely = low, sometimes = medium, often/always = high). I discarded the variables that had a very low response rate. 

Overall, this experience allowed me to learn more about data analysis and deal with real world data. Although I have experience with analysing data through programming, the dataset was often given to the class ready for analysis. I was able to learn how to deal with cleaning data, removing null values among formatting inconsistencies. I was able to learn how to use a new library in R that I hadn’t used before. 


## Data Analysis

To begin my data analysis, I created graphs to visualize the distribution of visitor agreement with the questions about their perception of the multimedia experiences in the museum (eg. did it make them discuss, enjoy more, feel inspired, learn, spend more time than expected, notice details they wouldn't have otherwise). I found that all of the variables are left skewed, with the majority of respondents agreeing with the statements. 

<div class="plot-grid">
  <img src="/assets/images/discussedDistribution.png"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/enjoyedMoreDistribution.png"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/feltInspiredDistribution.png"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/learningDistribution.png"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/moreTimeDistribution.png.png"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/noticedDetailsDistribution.png"
     onclick="openLightbox(this.src)">
</div>

<script>
function openLightbox(src) {
  document.getElementById("lightbox").style.display = "flex";
  document.getElementById("lightbox-img").src = src;
}
</script>




<div id="lightbox" onclick="this.style.display='none'">
  <img id="lightbox-img">
</div>
