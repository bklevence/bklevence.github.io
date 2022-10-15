---
title: "3D printers"
excerpt: "I'll pirate a car some day, mark my words."
toc: true
toc_sticky: true
header:
  teaser: assets/images/printers-00.jpeg
sidebar:
  - image: assets/images/printers-00.jpeg
    image_alt: "logo"
  - title: "Snapple Fact:"    
    text: "3D Printing started in 1985 by hand."
---

# FDM Printers

## How FDM 3D Printing Works.
For this example we'll use a Dimension ___ , manufactured by Stratasys. It is a Fused-Deposition Modeling system, and this is how it works:
After a 3D model has been designed and exported to an STL, a special program slices it up into cross-sections thick. It looks at each cross-section and generates a set of instructions on how to build it. When this information is sent to the printer, it starts with the bottom-most layer, laying down plastic in the shape of the cross-section. When it finishes the first layer, it moves up a slice to start on the next layer. Take a close look at a 3D-printed model and you'll notice that it is actually stepped.
The machine consists of a moving bed (Z-axis) and a print head (X-axis and Y-axis). The print head has a heating element in it; thermoplastic is forced into the print head, melts, and is squeezed out, not unlike toothpaste. The print head is calibrated in such a way that the molten plastic coming out of it is almost always the same thickness.
In order to form complex shapes, overhangs, and hinges/joints/free-moving objects, the plastic needs to be held up by something. The machine prints using a second material, which we call the 'support.' When the print is done, it is put in a bath of solution that dissolves away the support material, leaving only the finished model. Some machines do not have a second support material an instead have supports generated in the model material when sliced.

![Two Material, FDM Printing, Extrusion System Diagram](/assets/images/printers-01.png)

## Dimension

The Dimension SST 1200es I operated at UArts was a lemon. Material was the main culprit, but it was also an abused machine before I got to operate it. The 170 is okay, but when you print you're literally burning money.

## Ultimaker

**2+ Connect**

Quite a good machine. From my own experience with various printers, this is the buy. I'd get one for myself if I needed one!

## Lulzbot

### Overview

Great printers.
- [x] Lead Screws Lubricated (December 2019)
- [X] Need firmware updates.
- [ ] Material Sample Test for Tolerance
- [ ] Benchy off of each printer

### Printer Quirks @ NVD

**Printer 1**
- [ ] Y Belt Issues
- [x] Has some nozzle contact issues on calibration.
- [ ] Needs new PEI.

Tolerances for 1x1x1 cube test: X Y Z

**Printer 2**

- [x] Y Belt Issues
- [x] Has some nozzle contact issues on calibration.
- [ ] Needs new PEI.

Tolerances for 1x1x1 cube test: X Y Z

**Printer 3**

- [ ] Y Belt Issues
- [ ] Has some nozzle contact issues on calibration.
- [ ] Needs new PEI.

Tolerances for 1x1x1 cube test: X Y Z

**Printer 4**

- [ ] Y Belt Issues
- [ ] Has some nozzle contact issues on calibration.
- [ ] Needs new PEI.

Tolerances for 1x1x1 cube test: X Y Z

## Monoprice Maker Mini V2

Decent printer that I use at home directly off my PC with CURA. May set up Octoprint once I have a good location for the printer.

## Monoprice Maker Select

{% capture notice-warning %}
Run away from these fire-hazards. Even after fixing the thermistor...
{% endcapture %}
<div class="notice">{{ notice-warning | markdownify }}</div>

## Makerbot

### Replicator
Solid machine, likes loose extrusion, hard to keep consistent temp. Once it gets gremlins they stay.

### Replicator 2
Horrible machine, all I have interacted with have had ribbon cable gremlins. Run away.

### Replicator 2X
Really decent when they work. Can be very temper-mental. Does two materials well.

## Plastic Recycling Research

- [ ] Recycle Bot
- [ ] Precious Plastics

## Materials Review

- NGEN is great, but fractures, super shiny.
- PLA, good-old standard. Watch for moisture and dust.
- ABS, only for enclosed dimension, very susceptible to moisture damage.
- Ninjaflex, only used once. Can't use at home.
- TPU, want to try.

# SLA Printing

## Form 2?
Super interesting printer, not student friendly. I spent 2 months servicing one that a student almost broke the year before I got to NVD. Definitely get a good UV box or clean sunny space. There is actually a horrible design flaw in the spring connectors between the printer and the resin basin...

- [X] Inventory Material
- [ ] Write up checklist for proper handling

# Shapeways Printing

## Sandstone Printing
Done through shape-ways, link image from minecraft!

## Ceramic Printing
Done through shape-ways, link image from Ryans gift!




Notes that need to get added into above or gcode...

Working with Tolerance and Support Material.

There are a few basic guidelines to follow when developing a model for printing. These won't help you edit a model; these are things to keep in mind when designing it.

Wall Thickness - The printer can print walls as thin as ~0.01", however these will not be structurally sound. Keep walls to a minimum of 0.04" for rigid structure.

Suspended Parts - It is possible to make joints by leaving some space between two interlocking parts; leave at least 0.02" or the printer may connect the two parts. If a part is threaded or must fit snugly, it is best to print it separately (when possible).

Model Interior settings:

Solid: fills any interior space with 100% plastic. Strongest and most expensive option.


Sparse High Density: fills interior space with a grid pattern. Very strong and cheaper than Solid fill.


Sparse Low Density: fills interior space with a grid pattern using less plastic than Sparse High Density. Uses the least plastic and is therefore the cheapest.


Support Fill settings:

Minimal: uses the least amount of material and is therefore the cheapest option.


Sparse: uses more material than Minimal. Only necessary when printing complex overhangs or objects that require a high tolerance.


Printer Capabilities:
