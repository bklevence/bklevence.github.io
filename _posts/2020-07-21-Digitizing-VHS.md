---
title: "Digitizing VHS Tapes and MORE"
date: 2020-07-21 12:54
author: bklevence
---

***Digitizing VHS Tapes and MORE***

I've spent the last month resting after a tough semester implementing distance learning as well as finishing up my masters degree. In some of my free time I have been working on personal projects here and there. For my birthday my family gave me a little bit of money to go towards digitizing old home movie tapes (VHS, Hi8, MiniDV).

To start this journey I luckily had a Elgato EyeTV Hybrid already in my possession. I spent a few weeks combing eBay and finally snagged a Philips DVD Recorder/VCR DVDR 3545V. With these two devices I've been able to convert all VHS tapes while simultaneously dubbing DVD backups. I've also utilized the EyeTV Hybrid to record a .mp4 of each MiniDV tape [and will do the same for Hi8 once I find a camcorder].

The following is a digital procedure for digitizing and DVD Dubbing tapes using my setup. If recording from another device record as usual and follow conversion steps onward.

**Dubbing VHS->DVD**
- [ ] Place in VHS player and rewind.
- [ ] On Remote: SETUP -> RECORDING
- [ ] Set Dub to VHS -> DVD
- [ ] Autofinalize
- [ ] No Chapters
- [ ] Make Compatible (Still need isobuster)
- [ ] Put blank DVD into player
- [ ] Goto DVD
- [ ] On remote check REC MODE for dub type or length
- [ ] Set eyeTV buffer to 0 MB
- [ ] Press RECORD in eyeTV software
- [ ] Press DIRECT DUBBING on remote to begin VHS->DVD Dub.

**When Done**
- [ ] End recording on eyeTV
- [ ] Let DVD Finalize
- [ ] RW VHS
- [ ] Eject DVD and label immediately

**DVD File Rip(if eyeTV fails)**
- [ ] Load DVD into PC
- [ ] Open DVD in isobuster (paid software)
- [ ] Navigate to "Video.vob" and extract

**Converting Files**
- [ ] Either, find eyeTV recording in package contents of recording
- [ ] Or, find "Video.vob" extracted from DVD
- [ ] Open file in Handbrake
- [ ] Convert to .mp4 or .m4v, 480 Fast or Standard Quality is fine, HQ Surround is a pain when clipping videos for iOS

**Creating Chapters**
- [ ] Load .mp4 into Subler on OS X.
- [ ] Add chapters every 30 minute, then delete all but one
- [ ] Add chapters at times as needed, include titles
- [ ] Save to save chapters into .mp4

**Splitting Chapters into individual files for mobile or family sharing**  
- [ ] Open .mp4 saved from Subler in Handbrake
- [ ] Queue up conversions of specific chapters one at a time, Fast 480 is fine.
- [ ] Files will be saved as Title > Chapter Number unless settings are changed.
- [ ] Rename files as needed

Please note I have not found a good way to automate the last step of splitting a .mp4 based on chapters. Instead I'd rather spend my time just getting everything digitized. Let me know if you find a better solution!
