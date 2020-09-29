---
title: "GBA SP QI Charging"
date: 2020-08-06 12:54
author: bklevence
---

{% capture notice-danger %}
This is a draft!
{% endcapture %}
<div class="notice">{{ notice-danger | markdownify }}</div>

***GBA SP QI Charging***

**Disclaimers**

While I am a technology educator and have a degree in Industrial Design, I am not an Electrical Engineer!

Please note with the stock battery the battery door bulges a little, I don't mind it, but YMMV. This may also be fixed by using various battery mods or modifying(remove material) the case below the battery.

Utilize the exact same QI receiver I have used. Others have noted heat issues with other DIY QI kits. I have not had a problem with extreme heat, but the coil does warm up a little during normal operation. If you have to use another coil, test prior to enclosing it fully in the case.

I did this hack at my families summer cottage, so you should be able to do it with minimal tools.

**Impetus**

After updating the SP I began to fixate on updating the SP to be a contemporary device. Even newer "stock" batteries have horrific capacities, and I hate carrying around a cable for just the SP (and technically my 3DS). So I went to the internet and found out someone had done this previously behind the SP's screen. I wanted to do the same, but keep the device upright while charging!

**Research**

After viewing the tutorial above, and buying an octopus cable for my handhelds (GBC/SP/3DS) I realized that we're working with simple 5v ~.5A USB charging here. Also, thanks to those who've added micro USB or QI to their devices before me, it turns out it's quite easy to solder directly to the back of the vanilla charging port within the SP. This allows for the device to continue to control battery charging, is minimally invasive, easier than removing components or hijacking PCB traces, etc.

I made my way online and looked between amazon, eBay, and Adafruit for QI receivers for DIY hobbyists like myself. Amazon & eBay had many options, but would take forever on shipping. On Adafruit I realized I lucked out and they sell a QI receiver that supplies exactly what we need (~5v ~.5A). The PCB and coil also is flexi and more compact than other designs I was seeing.

It took about a week between requesting in-stock notification and it arriving at my door. Go Adafruit!

For folks in the EU [or those who want to get it cheaper], you may be able to find the same coil at other distributors or Aliexpress under the part name AK-QR200.


**Parts List**

- [ ] 30 AWG wire, can be bigger if you cut your case
- [ ] AK-QR200 Receiver (I bought two just incase)
- [ ] QI Charger (to test with)
- [ ] Soldering Iron (I use this cheapo one)
- [ ] Wire stripping tool (I used scissors)
- [ ] Tri-Wing(Nintendo) and Philips head screw drivers


**Procedure**

Remove Battery
Open up lower case and unfix the PCB

Cut two lengths of wire (more is better) and solder to pin 6(GND) and pin 3(PWR) (is this correct) on the rear of the power terminal. Note which wire is attached to pin 6 and pin 3 so you can properly match to Vout and GND on the QI PCB. I don't have two colors of 30AWG wire so I stripped the end of the wire on pin 3 longer so I could identify it as my PWR+ 5v wire to attach to Vout on the PCB after closing up the case.

Route wire down into batter compartment, screw PCB into case, and close case.

Place battery in case.

Begin to trim edges from QI coil shielding so it may fit better in battery compartment. You may remove it if you like, I chose not to.

Place QI coil and PCB above battery and trim edge of PCB if needed so that the battery door may close easily (see diagram below).

Figure out how long the wire needs to be to reach the GND and 5Vout pads on the PCB. Mark, cut, and strip the wire. Give yourself a little extra so you don't have too little wire.

Solder your wires to the central Vout and GND pads on the PCB as seen in the picture below. If your wires keep moving around use some tape to temporarily hold them. Take care in doing this as you have a battery directly underneath the PCB!

**Performance**

Stock Battery Testing (after roughly 5 charges/discharges):

With the IPS v2 at max brightness and an Everdrive x5 Mini on a stock battery I get roughly 55 minutes playtime until red light and about 15 minutes after that until the machine shuts off.

It takes roughly 1 hours to 1 hours and 20 minutes for the charging indicator to turn off using QI charging on an IKEA transmitter.

**Concerns**

Heat, especially with higher output QI receivers. I have charged and discharged the device multiple times and there is general warmth around the QI receiver after resting on the QI pad hours after charge completion. Not enough to be a concern right now, but I will keep an eye over time. I will note I cannot vouch for other QI receivers! Especially those with specs greater than 5V .5A and or including fast charging!

**TO DO**  
- [ ] Color code the 30AWG wire. (On Order)
- [ ] Battery swap, nondestructive way to get more space in battery compartment.
