---
layout: post
title: Spatial Tracking for Handhelds
excerpt: "Intrinsic and cheap external tracking for phones and tablets"
modified: 2014-11-27
tags: [HCI, Spatial, CHI]
comments: true
image:
  feature: tango.jpg
  credit: Project Tango
  creditlink: https://www.google.com/atap/projecttango/#project
---

# The superiority of dynamic peepholes
![spatial display](movePhone.gif)
In our [CHI 14 paper](www.mschuessler.de/pub/) we described a user study comparing spatial navigation using the peephole metaphor with multitouch: _"The results surpassed our expectations in various ways. On average, participants were more than **35% faster** with the spatial approach, even though all of them were conversant with Pinch-Drag-Flick and used the spatial technique for the first time. This finding was further supported by the questionnaires, where participants rated the spatial approach at least as good as or even better than the touch-based counterpart."_

# FAQ: _Why didn't you use the builtin gyro?_
![Opti Track](optitrack.jpg)
Ever since we showed our interactivity at CHI14 and the [IML Dresden](http://mt.inf.tu-dresden.de/en) Open Lab Days after ITS2014 inquisitive natures of various kinds have been looking at hour OptiTrack System (priced at more than 10k€) and wondered: _"Is that really necessary?"_

Various projects have used the gyro or the camera to track devices in space. Here are a couple of examples:
## Tilt to zoom
Apparently the Samsung S3 had a tilt to zoom feature - but if you think about it we need 6 DoF tracking and this is only 1 DoF.

<iframe width="560" height="315" src="//www.youtube.com/embed/Fb1JwWkk1hI?rel=0" frameborder="0" allowfullscreen></iframe>

### Sensor Fusion
There is a Google Tech Talk on fusing data of the intrinsic sensor and integrating accelerometer data, which will introduce you to the main problems you are facing when integrating over noisy data.

<iframe width="420" height="315" src="//www.youtube.com/embed/C7JQ7Rpwn2k?rel=0&t=23m8s" frameborder="0" allowfullscreen></iframe>

Microsoft research got very close to a solution. They build an image viewing application that adds face tracking to the input channel for sensory data. 
<video width="420" height="315" controls="controls">
<source src="http://research.microsoft.com/en-us/um/redmond/projects/lookingatyou/Video/LookingAtYou.mp4" type="video/mp4">
</video>

So you see we have to main problems here:
- noise
- latency

These to issues will influence the user experience and performance tremendously. Said in other words: you loose that 35% when you use one of the above solutions. So i am still waiting for someone to come up with a solution, so that we can get rid of the bulky OptiTrackSystem

# How long until we have device intrinsic spatial tracking?
The far most promising  Project Tango

## Cheaper external tracking
- Huddle Lamp
