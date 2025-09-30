---
title: "SSD Gauntlet" # Title of the blog post.
date: 2025-09-29T19:38:48-06:00 # Date of post creation.
description: "Performance testing of numerous M.2 Sata and PCIE SSD configurations!" # Description used for search engine.
featured: true # Sets if post is a featured post, making appear on the home page side bar.
draft: true # Sets whether to render this page. Draft of true will not be rendered.
toc: true # Controls if a table of contents should be generated for first-level links automatically.
# menu: main
usePageBundles: false # Set to true to group assets like images in the same folder as this post.
featureImage: "/images/path/file.jpg" # Sets featured image on blog post.
featureImageAlt: 'Description of image' # Alternative text for featured image.
featureImageCap: 'This is the featured image.' # Caption (optional).
thumbnail: "/images/path/thumbnail.png" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/path/share.png" # Designate a separate image for social media sharing.
codeMaxLines: 10 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: false # Override global value for showing of line numbers within code block.
figurePositionShow: true # Override global value for showing the figure label.
categories:
  - Technology
tags:
  - SSD
  - Homelab
  - Linux
# comment: false # Disable comment if false.
---

**Preface**

Hey! It's been a while! Fortunately, not long after working on my previous Terrarium Automation project blog posts, I was able to land a job supporting the USDA as a Senior Systems Administrator. Between being busy with that, and also spending a lot of time working on my new house as well as a project car (Honda CRX), I didn't continue work here on the site.

Well, here's to the revival of Curious Cyrus! One of the first reintroductions to this blog is goingto center on some at-home benchmarking and playing around with some flash storage!

**Testbench**
(Modified Dell T7910, Server Grade Workstation)

OS Kernal: CachyOS Linux 6.16.7-2 (64-bit) 

CPU: 2x Xeon  E5-2698 v3 (16 Cores x2) , 32 thread, 3.6ghz Turbo. 

Raid Controller: Dell Integrated (motherboard) LSI SAS 3008 12Gb/s SATA/SAS controller - SW RAID 0,1,10

PCIe Add-Ins: Asus Hyper M.2 PciE, 

RAM: 256GB (16x16GB) 2133MHz DDR4 ECC Memory, 8 Channels total

Cooling: Asus Hyper M.2 PciE using Aluminum Heatsin

**Preparation**
Temperature will be important when we consider how the drives perform, outside of pure transfer speed! This could be especially significant for longer testing, and real world applications where drives may have high utilization and ultimately get very few breaks! 

First, we will want to install psensor and hddtemp

```
sudo pacman -Syu psensor
sudo pacman -Syu hddtemp
```

Then, we'll run the below snippet to scan and issue detect/identify commands to all enumerable devices on the system. Here, we're especially concerned with the NVMe Devices. 

Read more about NVMe Identify/Scan commands from the Spec! A very useful tool for developers and learners alike, esentially a guideline for implementation and architecture dictation - https://nvmexpress.org/specifications/

Specifically, 

``` 
sudo sensors-detect 
```


```
sudo pacman -Syu nvme-cli
```