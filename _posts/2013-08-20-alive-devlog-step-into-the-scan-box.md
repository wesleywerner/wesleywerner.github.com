---
date: 2013-08-20
layout: changelog
project: Alive
title: "Devlog: Step into the scanbox"
description: ""
category: 
tags: []
---

This update is brought to you by protein muffins and digital frenzies.

![pixel cookie](/assets/alive/devlog/pixelcookie.png)

#### New screens

*   new help screens
*   main menu rework with save game slots and story selection

#### New widgets

*   GraphDisplay widget for showing health and power over the last few turns.
*   UxMovingButton widget for smooth sliding buttons.

#### New rendering

*   considers viewport offsets on various drawing calls
*   buttery smooth sprite movements
*   smooth viewport shifting
*   better support for drawing text paragraphs and blank lines
*   use DejaVuSansMono fonts
*   redraw the terminal and dialogue backgrounds

#### New interaction commands

*   @addcounter: add 1 to the object's internal counter.
*   @clearcounter: resets the object's internal counter to 0.
*   @setattr: alter the attributes of any objects within the containing rectangle.

#### New other things

*   lots of trace outputs - free bytes!
*   plot and level designs
*   our protagonist is now #00022 - what does it mean? it is a secret!
*   FAQ and map building doc updates

Screens
-------

A redesigned main menu, those buttons slide in and out as menus change:

![main menu](/assets/alive/devlog/alive-20130820-menu.png)

One of the update help screens:

![help screen](/assets/alive/devlog/alive-20130820-help.png)

The storage server room, lots of blinkenlichts:

![the server room](/assets/alive/devlog/alive-20130820-server-room.png)

The sick bay, for sick bots:

![sick bay](/assets/alive/devlog/alive-20130820-sickbay.png)

A terminal screen:

![a terminal screen](/assets/alive/devlog/alive-20130820-terminal.png)

