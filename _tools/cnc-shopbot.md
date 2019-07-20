---
title: "Shopbot CNC"
excerpt: "I have used both 48x48 and 96x48 PRSalpha models."
header:
  teaser: assets/images/shopbot-01.jpg
  toc: true
  toc_sticky: true
sidebar:
  - image: assets/images/shopbot-01.jpg
    image_alt: "logo"
  - title: "First Used"
    text: "2012"
  - title: "How it Works"
    text: "The CNC router is a milling machine outfitted with motors that precisely control each axis (CNC stands for Computer Numerical Control). It is a subtractive process which uses a moving spinning bit or cutter to cut through material. The bits of the router can be switched out; we have a range of bits. Material can be cut along two or three dimensions."
  - title: "Material"
    text: "Ply and hardwoods, MDF, masonite, acrylic, HDPE, LDPE, ABS, and foam (various densities)."
---

## 2-Dimensional Milling
The router follows vector lines. As with the laser cutter, these vector lines can be generated in Rhino, Illustrator, Onshape, or another CAD software. Since the bit has a diameter, you must specify how you want the machine to interpret your vectors. There are four options: *Inside, Outside, On The Vector, and Fill/Pocket.*

![Shop Scheduler](/assets/images/cnc-01.jpg)

### Inside:
the edge of the bit will hit the edge of a closed shape from the inside.

### Outside:
the edge of the bit with hit the edge of a closed shape from the outside.

### On the Vector:
the center of the bit will follow the vector

### Fill/Pocket:
the bit will completely remove the inside of a closed shape.

Since the machine has a Z-axis, you can specify how deep you want a path to be cut into the material. This is great for making dados or engraving graphics.

## 3-Dimensional Milling

The CNC router can also mill models from 3-dimensional files. For this to happen, the 3d file must be run through software that converts it into a set of instructions for cutting. It does this by analyzing the topology of the model and projecting a grid onto it. When cutting, the bit follows these gridlines (the distance between gridlines can be controlled, but is primarily based on the width of the bit). A basic diagram for the analysis of a 3d model along one axis:

![Shop Scheduler](/assets/images/cnc-02.jpg)

*A very important thing to note:* The bit is only capable of moving up and down; it doesn't rotate. This means that *undercuts are not possible*. Here is an illustration to clarify:

![Shop Scheduler](/assets/images/cnc-03.jpg)

### File Preparation

 <input type="checkbox" name="0" value="0">Units: inches
 <input type="checkbox" name="0" value="0">Layout board economically<br>
 <input type="checkbox" name="0" value="0">Check Offset/Cutter Tolerance for nested parts<br>
 <input type="checkbox" name="0" value="0">Within X and Y bounds for machine<br>
 <input type="checkbox" name="0" value="0">Within Z bounds, usually 0"-6" cutter depending.<br>
 <input type="checkbox" name="0" value="0">Join Vectors.<br>
 <input type="checkbox" name="0" value="0">Check fo duplicate lines.<br>
 <input type="checkbox" name="0" value="0">Create Layers.<br>
 <input type="checkbox" name="0" value="0">Assign Vectors to layers.<br>
 <input type="checkbox" name="0" value="0">Export Vector file for vector or 2.5D cuts.<br>
 <input type="checkbox" name="0" value="0">Export STL for 3D engraves.<br>


### Layer Naming Convention

- Cut_DepthOfCut_CenterofLine/InsideOfLine/OutsideOfLine_SpecifiedCutterDim
    >i.e Cut_750_CenterOfLine_250_EndMill (125 = ⅛”, 250 = ¼”, 500 = ½”, 750 = ¾”, 1000 = 1”)

- Drill_DepthOfDrill_SpecifiedCutterDim
- Engrave_DepthOfEngrave_DegreeOfVBIT
- Pocket_DepthOfPocket_SpecifiedCutterDim



{% include gallery caption="This is a sample gallery to go along with this case study." %}

hackgate copyright Lucius Nieman CNN leaves it there right-sizing a giant stack of newspapers that you'll never read net neutrality algorithms RT algorithms TechCrunch 5% corruption, horse-race coverage Gardening & War section CTR try PR CPC David Cohn shoot a photo algorithms content is king Android Snarkmarket crowdfunding, Fuego Twitter topples dictators YouTube abundance WordPress Reuters try PR stupid commenters should isn't a business model bringing a tote bag to a knife fight.
