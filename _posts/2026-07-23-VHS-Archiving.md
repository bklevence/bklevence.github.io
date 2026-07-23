---
title: "VHS Archiving: Clips & Chapters"
date: 2026-07-23 11:15
author: bklevence
---

***VHS Archiving: Clips & Chapters***

An update on my digital archiving project for my home videos!

My current workflow to produce clips for iCloud and chapterized videos to play anywhere:
1 - Start with cleanest video file(s) I can get
2 - Edit in Kdenlive
   - Import clips 
   - Best to render immediately so that you can do the next step cleanly, otherwise you poke around in settings far to much importing and exporting marker locations
   - Import full file or start fresh
   - Use automatic scene detection.
    - Threshold - 50 
    - Minimum Scene Length - 600 frames
   - Add start and end markers incase you must go to youtube eventually.
   - Edit, add, and name all markers how you like.   
   - Hopefully from this point you can just export everything, however if markers do not show up in export dialog do the following:
    - Export markers and re-import into primary "sequence" so they show up in timeline and not just clips, and make sure everything is aligned. You can just use the mouse in timeline to do this.   
   - Export out videos
    - MP4-H264
    [x] Markers Multi Export - All as separator
    [x] Deinterlacer - YADIF (better)
   - Export markers as TEXT file
3 - Open full video in LosslessCut
   - Import text markers textfile and check
   - Export video noted as chapterized

This took quite a bit of tinkering to get working on Linux, one of the big learning moments was installing all flatpacks through flathub. Prior to doing this I was having a crazy hard time getting Kdenlive, VLC, and most video programs to properly see FFMPEG for some odd reason. 

Next up items on my todo list:
0 - Get everything on a Flashdrive and eventually iCloud
   - Get proper metadata on individual clips before uploading and archiving.
1 - Figure out how to best use DVDStyler to make a DVD of the video with the chapters I've made

I almost wish I had a Mac to make the iCloud piece easer, but I think getting everything into my iCloud Photos library to share with family from my phone via flashdrive is easiest without introducing any new hardware to my life. 

Until next time!