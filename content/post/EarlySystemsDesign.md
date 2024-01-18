---
title: "Designing LEAP's Early Systems Architecture" # Title of the blog post.
date: 2024-01-18T11:51:55-05:00 # Date of post creation.
description: "Beginning diagrams for the main system and some encompassed subsystems" # Description used for search engine.
codeMaxLines: 30 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: true # Override global value for showing of line numbers within code block.
thumbnail: "/images/RemoteManagementDiagram.PNG" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/RemoteManagementDiagram.PNG" # Designate a separate image for social media sharing.
toc: true
figurePositionShow: true # Override global value for showing the figure label.
tags:
  - LEAP
  - diagramming
  - system design
  - blogging
--- 

# What does Early Systems Diagramming look like?:

In the realm of technology and software + hardware development, this process involves creating the initial diagrams for the main system and its encompassed subsystems! These diagrams have been created from my earlier post involving the Brainstorming of [LEAP](https://curiouscyrus.me/post/brainstorming/)

Further, I'd like to also delve into the significance of this phase and explore the facets involved in developing this evolving blueprint that will guide the rest of the development journey.

{{% notice tip "Tip" %}}
The Embedded Diagrams.NET can be zoomed in significantly to view any of the subsystems such as the Remote Management or Main Arbiter and Data-Link System!
{{% /notice %}}


<iframe frameborder="0" style="width:75%;height:597px;" src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&default-zoom=500&edit=_blank&layers=1&nav=1&title=LEAP%20Systems.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1KfchA9IXp2mdNBENvxPDNk0whlplhBI4%26export%3Ddownload"></iframe>


## Moving from the Foundation to the Architecture
When embarking on a new project, the first step is to conceptualize the main system. This involves outlining the core functionalities, identifying key components, and establishing the overall architecture.

This main system diagram acts as a roadmap, providing a visual representation of how different elements will interact and function together.

### Considerations for Integration:
In this early design stage, some consideration is given to how different subsystems should integrate into the main system. Power requirements, Compatibility, Data flow, and Communication protocols are defined to an extent. The aim here is to create the start of a well-coordinated system that will make logical sense!

## Iterative Refinement
It's important to also recognize that the initial design is a starting point rather than a conclusion. Iteratively improving and adjusting the diagram ensures the design will remain flexible with the project's evolving goals and requirements. Additionally, at this level there is still a level of abstraction and vagueness with respect to exactly how certain parts will function together that will get defined further as I work through milestones. 


## Conclusion
Architecting and Diagramming is a pivotal phase in any project's lifecycle. It lays the groundwork for the entire development process, providing a clear path for implementation. In navigating through the process of creating diagrams for the main system and its encompassed subsystems, I am intending to set the stage for a successful and well-orchestrated project. In the realm of design, these early systems are the blueprints that ideas into reality!
