---
layout: post
title: "Week 1"
date: 2026-06-14
---

In the first week of my internship at Mathaf, we focused on getting acquainted with the Museum and getting to know the visitors through observation and surveys. 

On the first day, we toured the collections of Mathaf and learned about its history. I learned that it began from the collections of Sheikh Hassan bin Mohammed bin Ali Al Thani and served as an artistic hub where artists took residency and made up most of Mathaf's early collection. 

On the second day, we visited the National Museum of Qatar to observe the visitors and collect data on their interactions with the multimedia components of the museum. Afterwards, we were to analyse the data through programming tools. I chose to use R. Although we were not able to gather much data due to the small number of visitors on the day we visited, we were able to use a larger dataset collected in 2023. 

During our tour of the National Museum, we learned not only about the history of Qatar but also about the ways it uses technology to enhance the visitor experience and how it was brought to life. The large wall projections in the Formation of Qatar and Natural Environments exhibits were created in partnership with Panasonic and utilizes numerous projectors to create high resolution images. In addition, the museum had interactive screens scattered through the space to display timelines and ultra high resolution images of displays that allow visitors to zoom in to see the most intricate details. 

In the data exploration section, I aimed to conduct a multivariate analysis to see the effects of different types of multimedia components in the museum to a variable like how much a visitor learns or how high they rate the experiences. I also wanted to add an interaction variable such as age range to see if the age of the visitors affected how much they learned from interactive screens. 

However, I found challenges with the data that made me simplify my approach. Firstly, not all questions were answered in the survey, which meant that each column had a different amount of responses. In this bar chart, we can see the number of responses per question:

![Responses Per Question](/assets/images/responses.png)

This caused a lot of the variables to have a very low sample size leading to an unstable model. Secondly, some categories had very few observations which makes it difficult to establish a clear relationship. For example, we cannot judge the impact of interactive touch screen use on learning if the data only shows some combinations (high use, high learning) and not others (medium use, low learning). The limited data in some groups make it hard to establish a pattern. The sparseness of the data also caused me to reject the idea of exploring an interaction variable, as the data already contains very small groups and introducing an interaction variable would only cause more issues. 

In the end, I was able to pivot by simplifying the data. For example, in the likert scale questions, I grouped strongly agree and agree together into one variable and strongly disagree and disagree together in another to limit the number of groups, especially since the data was already sparse. I also grouped behaviour variables together ( never/rarely = low, sometimes = medium, often/always = high). I discarded the variables that had a very low response rate. 

Overall, this experience allowed me to learn more about data analysis and deal with real world data. Although I have experience with analysing data through programming, the dataset was often given to the class ready for analysis. I was able to learn how to deal with cleaning data, removing null values among formatting inconsistencies. I was able to learn how to use a new library in R that I hadn’t used before. 

On Wednesday, we were introduced to a project Mathaf was working on in collaboration with google. Center Applied Imagination (CAI) that aims to connect scientists with artists to enable innovations through an AI lab. I am curious to learn more about the direction of the project and how it can impact the community. In addition, I am curious to learn more about the Mathaf Encyclopedia and how AI can be applied to create a database where the institutional knowledge of Mathaf can become more easily accessible to the public. 


