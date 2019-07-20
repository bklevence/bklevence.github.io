---
title: "Universal Laser ULS60"
excerpt: "I have used multiple ULS Models. Best CAM software."
toc: true
toc_sticky: true
header:
  teaser: assets/images/uls-01.jpeg
sidebar:
  - image: assets/images/uls-01.jpeg
    image_alt: "logo"
  - title: "How it Works"
    text: "The ULS VersaLaser is a 2-axis plotter, meaning it can move along the X and Y axes. The laser beam is focused through a lens, creating a focal point two inches below the lens where the beam is the most intense. In order to cut with the most precision, the focal point needs to be focused at the top of the surface it is cutting. For this reason, the laser is most efficient and precise when cutting sheet material."
  - title: "Material"
    text: "Ply and hardwoods, MDF, masonite, acrylic, select plastics, glass engraving, paper,"
---

## Diagram
This is a basic diagram of how the laser cutter works:

![Laser Diagram](/assets/images/laser-00.jpg)

## 3 ways to Process Material

![Cork Material Sample: Cut, Engrave, Raster](/assets/images/laser-03.jpg)

**Vector Cut:**
>Vector lines cut all the way through a material, and are drawn as red lines (R=255, G=0, B=0).

**Vector Engrave:**
>Vector lines that cut slightly into the surface of the material. It can be used to create text, graphics, or even texture on the surface of a material. Drawn as blue lines (R=0, G=0, B=255).

**Raster:**
>Dot Matrix engraving of a hatch or pixelated image onto the surface of the material using variable intensity. This allows a black and white image to be created, where 100% black translates to 100% laser intensity, and 0% black translates to 0% intensity. Left as solid hatches/fills or images and best set to grayscale.

Since the machine has a Z-axis, you can specify how deep you want a path to be cut into the material. This is great for making dados or engraving graphics.

## FAQs & Fun Facts

### Making things fit together (Tolerance)
- If you are cutting out parts using the laser cutter, getting them to line up/fit snug together/make perfect angles is tough. Here are some things to think about when designing a part.
### Plastics
- The diameter of the laser is about 1/100 inch, however some plastic will melt in the process of cutting (some cuts will appear wider than 1/100 inch as a result). Color can be a factor: because of the nature of light, white acrylic takes longer to cut than black acrylic (this is because white reflects a good amount of light from the laser while black absorbs most of it– the more a material absorbs, the hotter it gets). For most applications these things won't matter, but if a tolerance of above 1/16 inch is necessary, you should ask for a test cut with your material to make sure things go as planned.
- ***¡VINYL & PVC WILL CREATE CHLORINE GASS WHICH WAS USED IN WWI AS A CHEMICAL WEAPON!***
### Laser Drag and Material Thickness
- The laser doesn't cut through a material instantly. It takes a few milliseconds to get through a piece. The thicker the piece, the longer it will take. There is an effect called drag which can be seen on most laser cut pieces: since the top of the material gets cut first, the laser will spend more time cutting the top, producing a slight slope on the side of the piece. It is impossible to account for with the laser, so some hand-finishing may be required if a perfect 90 degree angle is desired.
- The slope will be more extreme with a thicker piece of material. For this reason we usually do not cut anything thicker than 3/8 inch (although it is possible and you should still inquire about it).
### Slots and Tabs (are tricky)
- If your parts are designed to be assembled using a slot/tab system, make a few test cuts first. Common problems with slots/tabs:
  - Shearing - If your slots and tabs are the exact same width and you try to jam two pieces together, they might snap. Especially if they are made of acrylic.
  - Material variance - Every sheet of plywood/acrylic/cardboard/etc. is slightly different. A perfect set of slots and tabs on one sheet might not translate well on another sheet. When possible, run test cuts on the same sheet(s) you'll be using for your parts.
  - Drag - Sloping sides can affect how well two pieces fit together. It is essential to do test cuts for thick materials (larger than 1/4 inch).
### Living Hinges
- I have [a small library of living hinges](http://steammetry.com/5-useful-living-hinge-template-for-your-next-laser-cut-project/), please see me for more info.

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

- CUT (Red)
- ENGRAVE (Blue)
- RASTER (Black)

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

[QuickStart Guide](/assets/docs/shopbot/quickstart.pdf){: .btn .btn--danger .btn--large}

- [User Guide](/assets/docs/shopbot/user-guide.pdf)
- [Command Reference v3](/assets/docs/shopbot/command-ref.pdf)
- [Feeds and Speeds](/assets/docs/shopbot/feeds-and-speeds.pdf)
- [Programming Handbook](/assets/docs/shopbot/programming-handbook.pdf)
- [Maintenance](/assets/docs/shopbot/maintenance.pdf)
- [Gantry Assembly](/assets/docs/shopbot/gantry-assembly.pdf)


## Weekly Checklist

  <input type="checkbox" name="0" value="0">Clean rack and pinions for X,Y and Z (2nd Z if present) with small brush and re-grease. Add a BB size blob of light grease every 6” and run the tool to its extents in all axes about 10 times. Wipe off any excess grease and recheck X & Y with push/pull test.<br>
  <input type="checkbox" name="0" value="0">Clean the Utilitrack (C channel rails on sides of PRS Z extrusion) with a solvent/lube like WD-40 and Scotchbrite pad. In high dust environments plastic rail wipers may have to be removed for proper cleaning of buildup. Wipe with light grease or machine oil.<br>
  <input type="checkbox" name="0" value="0">Scrub all hardened V rails with Scotchbrite pad saturated with WD-40. Wipe with clean rag. Remove dust covers and check V rollers for buildup and clean with small brass brush if needed.<br>
  <input type="checkbox" name="0" value="0">Add light machine oil to felt oilers inside of the 8 wheel covers and z-axis sweeps.<br>
  <input type="checkbox" name="0" value="0">Check rack/pinion/motor/shaft relationship by rapid push-pull. X1, X2, Y and Z. Adjust motor mount or tighten set screws.<br>

## Notes
- Swapped out control board twice on 48x48.
- Regrounded 48x48, feels like it has stuxnet. Random crashing/plunging...
- Redid Vac table on 48x48, ended up just switching to [plastic pneumatic nailer](https://raptornails.com/) to hold material to MDF spoilboard. Expensive, but worth it!
- 2016, UArts ID Shop 48x48 Machine was scrapped as it would not stop crashing.
- 2016, Workshop School needed dust collection, [I made an adaptor to standard ducting from original dust plate on 96x48](/assets/docs/shopbot/dust-attachment.zip).
