---
title: "Shopbot CNC"
excerpt: "I have used both 48x48 and 96x48 PRSalpha models."
toc: true
toc_sticky: true
header:
  teaser: assets/images/shopbot-01.jpg
sidebar:
  - image: assets/images/shopbot-01.jpg
    image_alt: "logo"
  - title: "How it Works"
    text: "The CNC router is a milling machine outfitted with motors that precisely control each axis (CNC stands for Computer Numerical Control). It is a subtractive process which uses a moving spinning bit or cutter to cut through material. The bits of the router can be switched out; we have a range of bits. Material can be cut along two or three dimensions."
  - title: "Material"
    text: "Ply and hardwoods, MDF, masonite, acrylic, HDPE, LDPE, ABS, and foam (various densities)."
---

## 2D Milling
The router follows vector lines. As with the laser cutter, these vector lines can be generated in Rhino, Illustrator, Onshape, or another CAD software. Since the bit has a diameter, you must specify how you want the machine to interpret your vectors. There are four options: *Inside, Outside, On The Vector, and Fill/Pocket.*

![Shop Scheduler](/assets/images/cnc-01.jpg)

**Inside:**
>The edge of the bit will hit the edge of a closed shape from the inside.

**Outside:**
>The edge of the bit with hit the edge of a closed shape from the outside.

**On the Vector:**
>The center of the bit will follow the vector

**Fill/Pocket:**
>The bit will completely remove the inside of a closed shape.

Since the machine has a Z-axis, you can specify how deep you want a path to be cut into the material. This is great for making dados or engraving graphics.

## 3D Milling

The CNC router can also mill models from 3-dimensional files. For this to happen, the 3d file must be run through software that converts it into a set of instructions for cutting. It does this by analyzing the topology of the model and projecting a grid onto it. When cutting, the bit follows these gridlines (the distance between gridlines can be controlled, but is primarily based on the width of the bit). A basic diagram for the analysis of a 3d model along one axis:

![Shop Scheduler](/assets/images/cnc-02.jpg)

*A very important thing to note:* The bit is only capable of moving up and down; it doesn't rotate. This means that *undercuts are not possible*. Here is an illustration to clarify:

![Shop Scheduler](/assets/images/cnc-03.jpg)

## File Preparation Checklist

 <input type="checkbox" name="0" value="0">Units: inches<br>
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

## Machine Preparation Checklist

 <input type="checkbox" name="0" value="0">Warm up spindle for 6-9 minutes with `[C][5]routine` (preferred) or 1⁄2 RPM if you do not have spindle speed control. Confirm operation of spindle fan.<br>
 <input type="checkbox" name="0" value="0">Check bit, collet and collet nut for wear and debris. Collets are good for 400-500 hours MAXIMUM of use if they are kept clean and no “event” occurs such as a broken bit inside the collet or a plunge that bottoms out on the collet.<br>
 <input type="checkbox" name="0" value="0">Check rack/pinion/motor/shaft relationship by rapidly pushing and pulling the carriages near each motor. X1, X2, Y and Z. Adjust motor mount and/or tighten set screws. A slight clicking sound should be heard, but no movement (over a few thousandths) should be present. Adjust if needed.<br>
 <input type="checkbox" name="0" value="0">Move the machine around the table in both jog and move speeds, or make a short warm up routine.<br>
 <input type="checkbox" name="0" value="0">Home the tool `[C][3] routine` using the prox switches.<br>
 <input type="checkbox" name="0" value="0">Zero your bit `[C][2]` (or other custom zero routine) to material surface or spoilboard.<br>
 <input type="checkbox" name="0" value="0">Verify that your bit has been zeroed properly by using a `MZ,0` command over the surface you have zeroed the bit to. Repeat zeroing if not correct.<br>
 <input type="checkbox" name="0" value="0">Perform a visual inspection of the machine, wiring, dust collection hoses and table surface. Verify proper operation of vacuum pump and dust collector (if present)<br>


## Guides & Documents


## Weekly Checklist

  <input type="checkbox" name="0" value="0">Clean rack and pinions for X,Y and Z (2nd Z if present) with small brush and re-grease. Add a BB size blob of light grease every 6” and run the tool to its extents in all axes about 10 times. Wipe off any excess grease and recheck X & Y with push/pull test.<br>
  <input type="checkbox" name="0" value="0">Clean the Utilitrack (C channel rails on sides of PRS Z extrusion) with a solvent/lube like WD-40 and Scotchbrite pad. In high dust environments plastic rail wipers may have to be removed for proper cleaning of buildup. Wipe with light grease or machine oil.<br>
  <input type="checkbox" name="0" value="0">Scrub all hardened V rails with Scotchbrite pad saturated with WD-40. Wipe with clean rag. Remove dust covers and check V rollers for buildup and clean with small brass brush if needed.<br>
  <input type="checkbox" name="0" value="0">Add light machine oil to felt oilers inside of the 8 wheel covers and z-axis sweeps.<br>
  <input type="checkbox" name="0" value="0">Check rack/pinion/motor/shaft relationship by rapid push-pull. X1, X2, Y and Z. Adjust motor mount or tighten set screws.<br>




{% include gallery caption="This is a sample gallery to go along with this case study." %}

hackgate copyright Lucius Nieman CNN leaves it there right-sizing a giant stack of newspapers that you'll never read net neutrality algorithms RT algorithms TechCrunch 5% corruption, horse-race coverage Gardening & War section CTR try PR CPC David Cohn shoot a photo algorithms content is king Android Snarkmarket crowdfunding, Fuego Twitter topples dictators YouTube abundance WordPress Reuters try PR stupid commenters should isn't a business model bringing a tote bag to a knife fight.
