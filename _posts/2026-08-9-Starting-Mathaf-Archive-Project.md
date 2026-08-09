---
layout: post
title: "Week 8: Starting the Mathaf Archive Project"
date: 2026-08-09
---
This week, we got started on the archives project that was brought up a few weeks prior. The goal is to build a program to help with the documentation of Mathaf's history. Currently, there are thousands of photographs, VHS tapes, and press clippings within the archive that have been digitized, but not labelled. A facial recognition program would help identify people in the photographs to speed up the documentation in comparison to manual labelling of all the thousands of photos. It would also be helpful to identify the artworks in progress in the backgrounds of these photos to link them to the completed artworks in the archive. A speech to text automatic transcription would make the tapes searchable and more easily summarized and labeled. 

# Sunday: Research

Before fully diving into the project, Iman and I decided to do research into how to actually implement the solution. We had both never worked on projects similar to this before so we worked on finding out how this could be done. I found a full tutorial on youtube by a creator named Nicholas Renotte, on how to build a facial recognition software for identity verification. He used Deeplearning with Tensorflow to train a model to recognize faces using a image dataset, meaning a set of faces that are not the target face to train the ai on what the person we want to recognize does not look like, an anchor image, meaning a picture of the target person we want to recognize, and positive images, meaning different photos of the target person in different lighting, angles, or expressions. 

This tutorial showed how to build the entire software from scratch, with 8 videos over an hour long each in the series. We decided this was not feasible given the time constraint of the project so we decided to look further. We found out we can use open source libraries of pretrained facial recognition software to build our application without starting from scratch. We decided to use Insightface, as it had the capabilities we needed, while being fully locally hosted, meaning that the images remain on the device and will not be sent out to any third parties. This was important to us, as it had been emphasized in previous meetings that the photos are not fully reviewed, so it is unclear what can and cannot be shared, and so all the photos are to be treated as confidential as of now. The downside of locally hosting is that there is a limit to the storage of our devices and therefore a limit to how many photos can be processed. 

There are other cloud based api that could have been used, such as microsoft azure that would have a larger capacity of processing of photos. However, these services requested payment. Although the Mathaf organization has access to Microsoft azure from their log ins, we cannot use it in our personal machines and our intern accounts do not allow us to log into the machines at Mathaf. 

# Monday

On Monday, we did not work on the Archive project, and instead did a showcase to the Mathaf staff of the robots. We demonstrated their capabilities and we received the SIM cards to allow them to have their own network connection. We spent the day on the showcase and trouble shooting some issues that came up. 

# Tuesday

After landing on Insightface as our software of choice, we started working on learning how to use it and how to implement our program with it. Idealy, we would have a knowledge base of each person. A folder for each person we would identify to compare with a new incoming image so that it can be identified. It would be structured as such:

### Person A
#### -IMG1.jpg
#### -IMG2.jpg
#### -IMG3.jpg

### Person B
#### -IMG1.jpg
#### -IMG2.jpg
#### -IMG3.jpg

Unfortunately, most of our images are unlabelled. The ones that are labelled, do not have each person specifically named. Some would have multiple people in a picture and labeled; "person A and person B working on project x." 




# Wednesday
Interface + Speech to text
# Thursday
Demo day

