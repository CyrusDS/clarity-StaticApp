---
title: "Brainstorming LEAP's Features" # Title of the blog post.
date: 2024-01-14T15:51:55-05:00 # Date of post creation.
description: "Brainstorming LEAP's Features" # Description used for search engine.
codeMaxLines: 30 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: true # Override global value for showing of line numbers within code block.
thumbnail: "/images/LEAPBrainstorming.png" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/LEAPBrainstorming.png" # Designate a separate image for social media sharing.
toc: true
figurePositionShow: true # Override global value for showing the figure label.
tags:
  - brainstorming
  - LEAP
  - blogging
---
<img src="/images/MindMapSmall.PNG" align="Center" width="1150" style="margin-right: 30px"/>

## Intro - Defining Components of LEAP: {style=text-align:center}
This post details the process I went through while working on the initial planning of the Paludarium, to organize and sort the possible scope of the Living Ecosystem Automation Project. 

This was one of the first times I used a Mind map, but I found it to help sort some ideas I had previously written down, but did not have collected in any meaningful matter to share. In working on this Mind Map, I was able to more clearly compartmentalize different sections of this overall large project, and visualize it in a way that makes sense - at least, to me! 

### Eight Main Components {style=text-align:center}
 Starting from the center of the Map, there are eight branches that I considered essential to the goals of the project. 
* Remote Management - This covers convenient methods of interfacing with the system, as well as addressing individual subcomponents through queries, or application based management. 
* Ecosystem Health Monitoring - Peripherals such as temperature or humidity sensors
* Terrestrial Management - Food and Water control for land-bound Flora and Fauna
* Aquatic Management - Food and Water Control for immersed life.
* Physical Features - How the actual Paludarium will look and the types of geographical features. This is less related to the Technological side of LEAP, but is a key component to having a realistic and beautiful environment.
* Custom Hardware, Physical Interfaces - This covers some of the more "completing" features beyond initial prototyping that I intend on including, such as custom PCB designs for microcontrollers, or hardware such as buttons.
* Ambient Features - This covers the "look and feel" of the Paludarium, bringing it to life, and adding some style.
* Photoperiodism - Lastly, another mandatory requirement for LEAP is to have proper lighting that covers the PAR [(photosynthetic active radition)](https://en.wikipedia.org/wiki/Photosynthetically_active_radiation) region of wavelengths and scheduling the lighting itself is paramount to thriving life. 

## About Each Component

### Remote Management
<img src="/images/RemoteManagement.png" align="center" width="950" style="margin-right: 30px"/>

What modern embedded system wouldn't be complete without an abundance of networking features and cross communication between different platforms? Automating in a modern way means being able to remotely access important features and options to control the system.

Plus, being able to share is important too! One longer term goal is to allow friends to visit a live stream of the Paludarium, and perhaps have an option to "Feed the Reptile" or cause a Thunderstorm for example.


### Ecosystem Health Monitoring 
<img src="/images/EcosystemHealthMonitoring.png" align="right" width="550" style="margin-right: 30px"/>

Most of the sensors are organized within this Monitoring section. At a high level, these system inputs will be used to help determine additional adjustments that may be needed in order to ensure the health of life within. 

For example, a low humidity may indicate that the system requires additional misting or waterflow to be delivered. 

Ultimately, most of the monitoring of may be contained to one embedded controller, which then reports to the main system which then issues commands to an appropriate output controller, such as the misting system.

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

### Terrestrial Management {style=text-align:center}
<img src="/images/TerrestrialManagement.PNG" align="center" width="850" style="margin-right: 30px"/>

Automatically providing sustenance for plants and animals will be handled through Auto Feeding and Auto Watering components. Irrigation wise, both a pumped misting system as well as a "Spray Bar" or "Drip Wall" will be implemented, providing moisture on the Paludarium background that plant life will enjoy.

I also want to include a Waterfall feature which can have its flow diverted via a servo, which could also reveal a hidden cave. This part is more of a "fun feature" 🙂

### Aquatic Management {style=text-align:center}
<img src="/images/AquaticManagement.PNG" align="center" width="850" style="margin-right: 30px"/>

In regards to aquatic life, such as immersed plants and fish, we must also ensure that the water quality is appropriate, and also have a method of dispensing food into the Water medium, instead of above land. 

### Physical Features
<img src="/images/PhysicalFeatures.PNG" align="left" width="650" style="margin-right: 30px"/>

Some of the more non-technical adventures on this blog will cover the creation of the physical features of the Paludarium. 

Between using Spray Foam to create a natural wall and painting it with Substrate, carving the flow of a small stream, or adding a sandy Zen Garden, I intend on adding some artistic and creative elements. 

I'm excited but also fairly anxious of this part of LEAP since I'll actually be a little more clueless on this sort of landscape creation and design!

I anticipate that I will likely go through multiple revisions for some of these elements as I get more practice 🙃

### Custom Hardware, Physical Interfaces
<img src="/images/CustomHardware.PNG" align="left" width="650" style="margin-right: 30px"/>

With some of my background in 3D Modeling and 3D-Printing, I intend on rapid-prototyping custom solutions to house and protect the hardware. 

Eventually, implementing PCBs designed specifically for each subsystem will be an end goal. Physically integrating a capacitive touch panel as well as a rotary knob will also allow users to check the system at a glance, or perform simple operations. 

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

### Ambient Features
<img src="/images/AmbientFeatures.png" align="center" width="850" style="margin-right: 30px"/>

Inspired by another maker who has been working on a nearly decade-long project of Automating his own Paludariums at https://paluweb.nl/ , I thought it would be awesome to be able to scrape web-data of the weather conditions in a particular area, then emulate those at my home. 

In other words, if Seattle had a drizzle all-day with a humidity of 70% and temperature of 68 degrees fahrenheit, then my home Paludarium would be automatically controlled to match this.

### Photoperiodism
<img src="/images/Photoperiodism.PNG" align="center" width="850" style="margin-right: 30px"/>

Lighting systems provide both the required energy for plants to thrive, while also raising the ambient temperature of the Paludarium. 

Ever go to an aquarium and see an exhibit which undergoes an adverse weather event? Having a FLASH of lightning, followed with subsequent delayed thunder from the Ambient Features, this would be a cherry on top as a part of the "feeling" of LEAP.

## Putting it All Together - Full Mind Map
<img src="/images/PaludariumPlanning.png" align="center" width="1050" style="margin-right: 30px"/>

And.. here's the entire Mind Map once complete! When viewed at this level, it's a fairly complete overview of the components of LEAP and what I intend on implementing. 

This does not, however, detail the priority, timelining, or other important considerations regarding the project. More than anything, this is a high level view to help break things down. 