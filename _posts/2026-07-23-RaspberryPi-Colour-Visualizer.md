---
layout: post
title: "Week 6: Raspberry Pi Colour Visualizer"
date: 2026-07-23
---

This week, our task was to build an interactive prototype using a single board computer called raspberry pi. 

# Sunday

On the first day, we focused on researching the raspberry pi and its capabilities, to then brainstorm ideas on what can be done with it in the context of the museum. My initial idea was to somehow use touch sensors and connect the pi to a museum api. The intention was to have different materials; canvas, wood, etc, which when touched would show artworks on the screen made with that specific medium. Another idea I had was to use the sensors as a different way to interact with a timeline. I was thinking of using the sensors as a touchless way to navigate through a timeline display. 

# Monday

On the second day, we received the devices; raspberry pi and arduino. We decided it would be best to get to know the devices and how to use it before we got started on building a prototype with it. We decided to follow a tutorial on how to use a distance sensor with the raspberry pi. 

![Distance Sensor](/assets/images/distanceSensor.jpg)

We watched videos and read written tutorials and tried our best to follow the wirings, but in the end we were not able to get it to work by the end of the day. 

# Tuesday
The following day, we decided to use the rfid card reader instead of the distance sensor, as the wirings had already been on the device originally, so it was easier to set up. We placed the wires on as needed and got started on connecting the raspberry pi to a screen and keyboard to begin coding. At first, we began by trying to connect the rapberry pi to a laptop via HDMI, but it was not working. There was no display appearing on the screen. We then tried using the office monitor at mathaf, but we were also not able to make it work. The computer was attached to a cpu that runs a specific device. When the cpu was disconnected, there was no HDMI plug on the monitor itself, so it could not be used. Finally, we used the small touchscreen device included in the kit. It was able to show the display, but we were unable to code with it because we couldn't type. We then figured out that we could use the keyboard in the office to type with via a USB connection. On this day, we were able to get the cards to scan on the RFID sensor. 

<div class="two-grid">
  <img src="/assets/images/RFIDSensor.jpg"
     onclick="openLightbox(this.src)">
  <img src="/assets/images/RFID.jpg"
     onclick="openLightbox(this.src)">
</div>


# Wednesday
On the fourth day, we decided to start rethinking what we could do with the device as a prototype, as we were finally able to get the device working. We had an idea to place IDs or tags inside sample artworks and display them as replicas. Users would then be able to scan these mini artwork replicas to see a full bio of the artist who made it and details on the artwork, as well as other works by the artist. Christophe suggested that something that could connect the books to online or gallery collections would be a good idea. 

From here, we thought it would be a good idea to be able to scan a book and view all the artworks included inside it, as well as the dominant colours in the works. After some brainstorming and taking into consideration projects we did in the past, we decided a good product might be to see trends in colours in the works over time. We decided a good way to show this would be to plot the dominant colours of an exhibition on a colour wheel. We could plot the dominant colours of each past exhibition on its own colour wheel to see the tendencies of colour use in each one, maybe a lot of yellow in one, or a lot of red in another. 

Since we did not have access to a list of artworks in each exhibition with high quality images, what we ended up doing is borrowing one book, Sajjil: a century of modern art, and using it as an example. We manually took pictures of a sample of artworks from the book, wrote the attributes in a csv format, and decided to use the categories within it as sections rather than by exhbition. We plotted works from the family section, from the nature section, and the city section to see the differences. 

# Thursday

The majority of Thursday was spent on the development of the website, as well as creating our data (taking pictures and writing down the attributes in an excel format). We decided to use a shared github repository to work on it collaboratively together. We thought we could develop most of the app on our personal devices then just clone the code into raspberry pi later. Although the app was not as polished as we would have liked by the end of the day, we decided to move on to running the app on the raspberry pi. We found that we were able to run the wensite, but it was more difficult trying to connect the rfid sensor to our code. We wanted to have each card represent a section in the exhibition, so that the user could scan a card to see the colours plotted on the colour wheel. However we were not able to implement that part, so only the buttons work. 

![Finished Page](/assets/images/exhibitionPalette.jpg)


<script>
function openLightbox(src) {
  document.getElementById("lightbox").style.display = "flex";
  document.getElementById("lightbox-img").src = src;
}
</script>
