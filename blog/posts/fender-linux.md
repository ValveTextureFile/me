---
title: linux w/ fender mustang lt25 amp support type thing
date: 2026-09-16 23:57:05
slug: fender-linux
description: HID stuff, protobuf, and a Mustang LT25
---

i currently have a Fender Mustang LT25 guitar amplifer that I also use for my bass, and I started to wonder:
> how could i possibly control my amp on my arch desktop?

so i lowk got to work

## finding the amp

quick lsusb and udevadm lead me to getting the vendor and product id of the amp:
```text
VID: 1ed8
PID: 0037
interface: 0
```

there is this awesome guy i found while researching the communication layer between the amp and Fender Tone (the standard desktop app that fender provides for controlling the amp.), and he made protocol buffers for the Fender Mustang LT25 anyway, so that was a **RELIEF** that i dont have to touch ghidra for reverse engineering.

The repo is [here](https://github.com/brentmaxwell/LtAmp) if you wanna look at it. its a neat lil c# library + app which i find great.

## current progress report

its actually doing pretty well ngl.

other than the fact i need to study to get my SAT score up the project itself is going well.

right now as i write, the project (guit2. i came with it on the spot dont ask might change later) is done with communcations from host to amp, and now needs to get a syncing state done so i can make a middle ground between the front and back end for the amp presets.

