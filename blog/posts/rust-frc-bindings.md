---
title: im making frc bindings for rust...
date: 2026-09-20 
slug: rust-frc-bindings
description: a little side project, not completly replacing guit2
---

## okay people get bored
we all get bored, so im turning away from `guit2` for a little bit and working on `rplib`, robot programming library, which is a rust library for FRC (FIRST Robotics Competition). It will probably look good on the apps, but im doing this because i want:
1. more flexible language options for WPILib.
2. more challenge.

## what i did so far
right now i can get HALsim to run with bindings made from bindgen, which is fun, so that part's down.

so far, i have a higher level struct for digital output so i can do some test stuff, nothing too serious yet.

im working on getting local halsim to work cross-plat, so i need to download wpnet, -math, -util, nicore, etc.

anyways thats pretty much it. project aint even in working stage yet execpt for bindings. if you would like to check it out, here is the [repository](https://github.com/ValveTextureFile/rplib).


