---
title: "Stinger SR23 CNC"
excerpt: "CAMaster has the best CAM workflow."
toc: true
toc_sticky: true
header:
  teaser: assets/images/sr23-00.jpeg
sidebar:
  - image: assets/images/sr23-00.jpeg
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
 <input type="checkbox" name="0" value="0">Check for duplicate lines.<br>
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

## CUT2D Checklist

<input type="checkbox" name="0" value="0">Material Measured w/ Caliper<br>
<input type="checkbox" name="0" value="0">Material Size<br>
<input type="checkbox" name="0" value="0">Can be clamped?<br>
<input type="checkbox" name="0" value="0">Join Vectors<br>
<input type="checkbox" name="0" value="0">Vectors on right Layers?<br>
<input type="checkbox" name="0" value="0">Begin making Toolpaths<br>
<input type="checkbox" name="0" value="0">Check tool<br>
<input type="checkbox" name="0" value="0">Specify tab locations<br>
<input type="checkbox" name="0" value="0">Generate<br>
<input type="checkbox" name="0" value="0">Repeat for other processes.<br>
<input type="checkbox" name="0" value="0">Simulation Preview<br>
<input type="checkbox" name="0" value="0">Check tab and nesting tolerances<br>
<input type="checkbox" name="0" value="0">Generate TAP files.<br>

## WINCNC Machine Preparation Checklist

<input type="checkbox" name="0" value="0">Initialize<br>
<input type="checkbox" name="0" value="0">Measure Tool<br>
<input type="checkbox" name="0" value="0">Touch Top Zeroing Command<br>
<input type="checkbox" name="0" value="0">Laser ON<br>
<input type="checkbox" name="0" value="0">Jog around and Zero to Laser<br>
<input type="checkbox" name="0" value="0">Open .TAP File<br>
<input type="checkbox" name="0" value="0">CTRL + V to preview<br>
<input type="checkbox" name="0" value="0">FILE>SIMULATE (Z should only be RED)<br>
<input type="checkbox" name="0" value="0">Turn Spindle ON<br>
<input type="checkbox" name="0" value="0">Enter to start<br>

## Guides & Documents (needs files)

[QuickStart Guide](/#){: .btn .btn--danger .btn--large}

- [User Guide](/#)
- [Command Reference v3](/#)
- [Feeds and Speeds](/#)
- [Programming Handbook](/#)
- [Maintenance](/#)


## Weekly Checklist

  <input type="checkbox" name="0" value="0">Clean rack and pinions for X,Y and Z (2nd Z if present) with small brush and re-grease. Add a BB size blob of light grease every 6” and run the tool to its extents in all axes about 10 times. Wipe off any excess grease and recheck X & Y with push/pull test.<br>
  <input type="checkbox" name="0" value="0">Clean the Utilitrack (C channel rails on sides of PRS Z extrusion) with a solvent/lube like WD-40 and Scotchbrite pad. In high dust environments plastic rail wipers may have to be removed for proper cleaning of buildup. Wipe with light grease or machine oil.<br>
  <input type="checkbox" name="0" value="0">Scrub all hardened V rails with Scotchbrite pad saturated with WD-40. Wipe with clean rag. Remove dust covers and check V rollers for buildup and clean with small brass brush if needed.<br>
  <input type="checkbox" name="0" value="0">Add light machine oil to felt oilers inside of the 8 wheel covers and z-axis sweeps.<br>
  <input type="checkbox" name="0" value="0">Check rack/pinion/motor/shaft relationship by rapid push-pull. X1, X2, Y and Z. Adjust motor mount or tighten set screws.<br>

## Notes
- Had two controller issues. Both required hardware swap.
- Was crashing into zero plate and measuring tool, was loose cable.

- [ ] Find docs on 3D
- [ ] Work on clamping to edge.
- [ ] Feeds and Speeds / Cut depth for faster Ply cuts.
- [ ] Get Manuals of PC for both CUT2D Pro and WinCNC.
- [ ] Zero on spoilboard rather than top of material?
