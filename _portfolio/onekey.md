---
title: "OneKey"
excerpt: "Low cost digital hardware fabrication for makerspaces"
toc: true
header:
#  image: /assets/images/unsplash-gallery-image-2.jpg
  teaser: assets/images/ok-teaser.jpg
sidebar:
  - title: "UArts Capstone Project"
    image: assets/images/ok-sidebar.jpeg
    image_alt: "logo"
    text: "2014"
  - title: "Materials"
    text: "3M Copper Tape, PCB Blanks, Hobbyist Electronics"
  - title: "Tools"
    text: "Vector Editors, Vinyl Cutters, Eagle, OSH Park"
---

>[Hop on over to Github to see the full documentation of the current iteration of the oneKey, below is directly lifted from the repo.](https://github.com/makerjawn/oneKey/)

Project Focus
-------------------
Developing a low-cost (<$2) and accessible derivative of the MaKey MaKey so that it can be sustainably deployed via workshops at various library branches.

The aim is to introduce youth in underserved/low-income communities to making hardware that they can then tinker/play/make with. It's adressing the question "Can I take this home?" and the inability for youth to use take projects using digital media tools such as the MaKey MaKey home.

In participating in this process we hope for them to take more ownership of their tools. We're also trying to adress wether or not the library and its participants can make their own tools for learning via desktop manufacturing and production methods.

So what is a MaKey MaKey?
-------------------
From Sparkfun's [*MaKey MaKey Documentation*](https://github.com/sparkfun/makeymakey):

*"Using the MaKey MaKey you can make anything into a key (get it?) just by connecting a few alligator clips. The MaKey MaKey is an invention kit that tricks your computer into thinking that almost anything is a keyboard. This allows you to hook up all kinds of fun things as an input."*

**How does it work?**

*"The MaKey MaKey uses high resistance switching to detect when you've made a connection even through materials that aren't very conductive (like leaves, pasta or people). This technique attracts noise on the input, so a moving window averager is used to lowpass the noise. The on-board ATMega32u4 communicates with your computer using the Human Interface Device (HID) protocol which means that it can act like a keyboard or mouse."*

Methods
-------------------
The original oneKey uses a vinyl cutter and 3M copper tape to make a low-barrier and low-cost method for creating traces to solder onto. If working indoors take precautions with ventilalation etc. Working currently on a PCB kit version.

Brief History
-------------------
To date two iterations of the one input MaKey MaKey derivative, "MaKey MaKey MaKey", or officially "oneKey" for short, have been deployed. The first generation proved that youth could make, hack, and play with their own hardware. After various form and material explorations as well as a circuit redesign it is currently in its second phase. The new design is easier to handle, the cost per unit has dropped from $7 to $1.30, it's quicker to make, and there is still much more to refine.

Variations
----------------
**Vinyl Cut Copper Tape**

![oneKey Vinyl](https://farm8.staticflickr.com/7500/16254418821_7e90b29a9c_b.jpg)

This build requres soldering and takes an hour to construct. The tape can be tricky to adhere to a substrate, but for all intents and purposes IT WORKS!

Requires the installation of the Digispark Arduino IDE to upload and run code from /Firmware.
All vector files needed for vinylcutting reside in /Hardware.

**PCB(REV.1)**  

![PCB](https://i.imgur.com/47suY3K.png)

![PCB2](https://i.imgur.com/VneJiBF.png)

Looking to make a PCB kit, currently waiting for PCB to be milled. See the Eagle Schematics and Board files in /Hardware.

**Quick-build(Still in Development)**  
This build is solderless, can be built in less than an hour.
