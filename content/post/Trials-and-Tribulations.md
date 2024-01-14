---
title: "Trials and Tribulations of Website Hosting" # Title of the blog post.
date: 2024-01-13T15:51:55-05:00 # Date of post creation.
description: "Exploring the workflow for designing and hosting a Static website for blogging" # Description used for search engine.
codeMaxLines: 30 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: true # Override global value for showing of line numbers within code block.
thumbnail: "/images/AzureThumbnail.png" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/AzureThumbnail.png" # Designate a separate image for social media sharing.
toc: true
figurePositionShow: true # Override global value for showing the figure label.
tags:
  - Web-dev
  - Azure
  - Cloud
  - blogging
---
## Intro: {style=text-align:center}
This post details the process I went through while working on this Blog website and ultimately hosting it here at https://curiouscyrus.me/

For more information on why this blog exists, and the content on it, see [What is LEAP?](https://curiouscyrus.me/post/starting-a-project/) You can also find the accompanying public repository for my Web app [here](https://github.com/CyrusDS/clarity-StaticApp) as well! 

## Deciding on the Type of Website {style=text-align:center}
One of the first steps on my Website creation adventure was to determine the type of website that would be suited for my specific application. For this Website, I wanted a blog-style interface which would allow sufficient customization with site organization while also keeping things simple in terms of adding new content to the Website

In this case, I also have no need to store any user data or perform complicated operations that would require real time updates, and the priority is to provide a quick and snappy experience.
<img src="/images/Static_vs_dynamic.jpg" align="Center" width="850" style="margin-right: 30px"/>

Therefore, the most appropriate type of website was a Static Website. The next steps were to determine a Website Framework to use, or whether to start from scratch!

## Website Frameworks - Hugo
<img src="/images/Hugo_MDown.png" align="Center" width="550" style="margin-right: 30px"/>

[Hugo](https://gohugo.io/getting-started/quick-start/) allows you to write pages for websites with __Markdown__, which was a major factor in why I decided to go with it. Partly, my goal for this Website and Domain is to display educational posts - therefore, being able to easily add posts in a simple formatting is ideal! Having worked with LaTeX in courses previously.. and not being a huge fan, Markdown is a nice switch!

I also figured with the widespread applicability of Markdown as a practical documentation method, I oughta' get some practice 😉

### Installing [Hugo](https://gohugo.io/getting-started/installing)
* Working with Hugo is fairly straightforward, though, when it comes down to customizing your website - there are a few nuances based on your Theming choices.. more on this later!

For my Windows system, I used [Chocolatey](https://chocolatey.org/) and while running an admin powershell, install simply required 
```
  choco install hugo 
```
### Theming.. and Re-Theming...

The Hugo tutorial uses the Ananke theme, which I initially worked with while evaluating the feasibility of Hugo itself, and whether I was going to continue to run with it when making this Website!

Before looking at hosting the Static Website I made in a few minutes with Hugo, I ran the local instance via 
```
  hugo server
```
I customized a few elements on the default theme, such as the background color, experimented with adding a post or two, and looked at some of the options you can customize via the built in *hugo.toml* files.

<img src="/images/hugo-toml.PNG" align="Center" width="550" style="margin-right: 30px"/>

After evaluating that Hugo seemed sufficient while visiting some friends in WA, I commited the initial repository to save my work and then visit a few days later when I would be back in Colorado.
In the mean time, I was interested in looking at some of the public options on the themes [subpage](https://themes.gohugo.io/) of Hugo and found [Clarity](https://themes.gohugo.io/themes/hugo-clarity/#custom-css-and-js) which caught my eye much more.

<img src="/images/Curious-Ananke.PNG" alt="An early test revision of the Website" align="Center" width="750" style="margin-right: 30px"/>
One major thing to note about themes in Hugo though, is that each Theme has its own subset of parameters and conventions which influence how the HTML and CSS is built and then subsequently displayed. In switching to Clarity, I did have to essentially re-orient myself with the Framework. 

![::img-center img-shadow](/images/toml-files.PNG)

In the case of Clarity, one unique feature is that the regular *hugo.toml* file that I mentioned earlier, is actually unused. Instead, it has been re-implemented as a set of *.toml* files within the _\config\_default_ folder. 


I find this method to provide greater customization, and also found it to be fairly intuitive, for example you can see the Header menu bar being configured below in the *.toml* for the menu. 


<img src="/images/toml-menu.PNG" align="Center" width="550" style="margin-right: 30px"/>

```
[[main]]
  name = "Home"
  url = ""
  weight = -110

[[main]]
  name = "Videos"
  url = "post/rich-content/"
  weight = -105
[[main]]
  name = "What is LEAP?"
  url = "post/starting-a-project/"
  weight = -107
```

Technically, this is the menu in English, since Clarity provides support for language switching. Sadly, I'm not a polyglot, and my French is a bit rusty so I am not using this feature 😅

There are plenty more customizations I made to adapt the base Clarity theme to my goals and intents, including adding a CSS override file to change the background colors when building the site, which is output to the *public/* folder

## Choosing a Hosting Method - Microsoft Azure: Cloud Computing

## Github Workflow and CI/CD

## Purchasing and Using a Domain

## Google Analytics and More