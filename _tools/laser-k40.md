---
title: "K40 Laser"
excerpt: "Check the grounding 5000 times, then cut."
header:
  teaser: /assets/images/k40-00.jpg
sidebar:
    image: /assets/images/k40-00.jpg
    image_alt: "logo"
  - title: "Material"
    text: "1/8 Ply, acrylic, paper, tortillas"
---

I bought one of these for roughly $400 to learn more about laser cutters after having rebuilt a Full Spectrum Laser. You must also buy an air assist if you want to cut anything properly. I suggest getting it as cheap as possible and use light-object for all upgrades. You must also buy a pair of laser safety glasses to safely operate around.

I almost never run this thing regularly so below I am only listing the set-up steps for my own usage. If you'd like to learn more about lasers see VLS.60 or Epilog tool pages.

## Machine Preparation Checklist

 <input type="checkbox" name="0" value="0">Check Grounding on outlet and K40.<br>
 <input type="checkbox" name="0" value="0">Prime Pump w/ 3 Gallons Distilled Water.<br>
 <input type="checkbox" name="0" value="0">Vector SVG, can have normal color conventions.<br>
 <input type="checkbox" name="0" value="0">Install CorelDraw & CorelLaser<br>
 <input type="checkbox" name="0" value="0">Open in CorelLaser (less buggy)<br>
 <input type="checkbox" name="0" value="0">Check Alignment w/ Test fire.<br>
 <input type="checkbox" name="0" value="0">Exhaust On<br>

- [Corel Template for Laser](/assets/docs/k40template.CDR)

## First run

Much of this material is thanks to [k40laser.se](https://www.k40laser.se/).

Open CorelLaser. Use the template, it has one engraving layer and one cutting layer. When CorelLaser is installed you will find the menu below. Click on the green pen icon.

  ![Laser Diagram](/assets/images/k40-01.jpg)

Control settings so its identical to this screen.

  ![Laser Diagram](/assets/images/k40-02.jpg)

Most important setting is the mainboard, you may need to change this later if your machine operates very slow (a first sign of wrong mainboard selected)
You can find information about which board you have on the controller board in your machine.

  ![Laser Diagram](/assets/images/k40-03.jpg)

Next setting is to check your hardware device ID, you can find this on the controller board, se image below

  ![Laser Diagram](/assets/images/k40-05.jpg)
  ![Laser Diagram](/assets/images/k40-06.jpg)


Check out the other settings and make sure you have the same on your settings.

  ![Laser Diagram](/assets/images/k40-07.jpg)


You are now ready to start your first test with the machine
Start with the “rectangle tool” in corel, make a box with the size of your choise, i made a 54x40mm box.

  ![Laser Diagram](/assets/images/k40-08.jpg)

Select the box as shown in the picture, and in the top menu you see a line width set to “hairline”.
Change this to 0.001 and hit enter.

  ![Laser Diagram](/assets/images/k40-09.jpg)

You are now ready for your first cut test.

Select CUT in the corel menu, the icon marked here

  ![Laser Diagram](/assets/images/k40-10.jpg)

Click OK on the data setting, we did this in a earlier step.
Make sure the settings are still there.

Now you have this setup box (click to expand)

  ![Laser Diagram](/assets/images/k40-11.jpg)

To explain some of the settings
Company and model is just the data about your machine.
Rotate: if you need to rotate or flip your design for mirrored cut/engravings.
Style: Cutting, engraving and marking. For this test we choose CUTTING.
Inside first is a good option if you make parts, the machine will cut the inner parts first and then the outer, preventing the part to fall down without the inner holes are cut.
Speed: I have a 3mm acrylic piece in my machine, you may have to test the speed and the power on your machine when testing your cut.
I would suggest 12mA power and 10mm/sec to start with.
Method: If you have combined engraving and cut in the same file, you can choose here.
In the template before, we split engraving and cut in two different layers, this will help you to run the engraving first, and cut later.
Pixel: set this to 1 step, and Repeat to 1 times

You are now ready to hit STARTING

More tips and tricks
Test similar design to learn how power and speed relates on your machine, this is different on most K40 and you cannot use the same settings someone else has. You need to find your optimal combo
