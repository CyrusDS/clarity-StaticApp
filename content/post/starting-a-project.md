---
title: "LEAP - A new initiative" # Title of the blog post.
date: 2024-01-07T15:51:55-05:00 # Date of post creation.
description: "When an idea becomes a plan, then a plan becomes action" # Description used for search engine.
codeMaxLines: 30 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: true # Override global value for showing of line numbers within code block.
thumbnail: "/images/starting-thumbnail.png" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/starting-thumbnail.png" # Designate a separate image for social media sharing.
toc: false
figurePositionShow: true # Override global value for showing the figure label.
tags:
  - LEAP
  - blogging
  - web dev
---
<img src="/images/largetank.jpg" align="right" width="400" style="margin-right: 30px"/>

# So, what exactly is this??
## LEAP - Living Ecosystem Automation Project
LEAP is a project I have been slowly building a plan together for since as early as 09/26/2023 when looking to incorporate water and land elements in a living ecosystem, after becoming inspired by some excellently designed enclosures that other hobbyists have designed in recent years. 

Eventually, this morphed into something where I wanted to combine my skills and knowledge in Embedded Systems design with a goal of creating multiple subsystems run by specialized microcontrollers, which could vary between irrigation controls, livestreamed camera feed, humidity tracking, and much more. 

Additionally, these subsystems would be designed such that they report to an underlying main processing system, running on a Real-Time OS, handling queries in a task oriented style. For this to be most convenient, such an automated system also needs to be able to interface to a network so that all data streams can be accessed in real time and so the system itself can respond to queries sent by an Administrator (That's me!)

# What the heck is a Paludarium?

<img src="/images/threetanks.jpg" align="right" width="400" style="margin-right: 30px"/>

[Terrariums](https://en.wikipedia.org/wiki/Bioactive_terrarium), [Vivariums](https://en.wikipedia.org/wiki/Vivarium), or [Paludariums](https://en.wikipedia.org/wiki/Paludarium), are all semi or fully enclosed systems have a multitude of qualities which are essential to properly maintaining the health of the entire biome. 
* ###### Check [here](https://terrarium.blog/en/explanations/terrarium-vivarium-paludarium-difference/#:~:text=In%20a%20paludarium%2C%20amphibians%20and,do%20not%20have%20to%20be.) to find out more about the differences between these three types of "ariums" 

&nbsp;

## Where does Automation come in?

<img src="/images/EcosystemHealthMonitorDiagram.PNG" alt="Example diagram of LEAP's sensing system." align="center" width="1100" style="margin-right: 30px"/>

\

See more of the System Diagram [Here](https://curiouscyrus.me/post/earlysystemsdesign/)

In order to ensure ideal conditions that would allow the flora, fauna, as well as underlying micro-organisms to thrive, there is a significant value to automatically adjusting (our controlled) environment in response to measured biological indicators of health.

Methods to determine this can vary from the precise monitoring and control of the enclosed system's humidity, temperature, soil and water pH, as well as many more crucially important aspects such as adaptable scheduling for lighting and water distribution. 
* (See project index and breakdown for further information on the overall system design and sub-projects encompassing this entire automation task! Between CAD, PCB design, web dev, embedded RTOS, investigations into communication protocols, and MUCH more, there is a lot to check out!) 

Having such closely related but independently controlled sub-systems allows these components to be encapsulated within dedicated embedded systems that can then be controlled by an underlying master through a common communication protocol. 

###### Overview last updated - 01/10/2024