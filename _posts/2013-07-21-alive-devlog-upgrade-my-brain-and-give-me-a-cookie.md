---
date: 2013-07-21
layout: changelog
project: Alive
title: "Devlog: Upgrade my brain and give me a cookie"
description: ""
category: 
tags: []
---

Today's post is brought to you by strawberries and neural upgrades.

![pixel cookie](/assets/alive/devlog/pixelcookie.png)

notable changes
---------------

*   resized the tileset. allows for more animations.
*   create a new level 1 and 2 with story and humor.
*   create a tech demo map, showcasing engine features.
*   use different dialogue backgrounds for "terminal" and "story" types.
*   the ui buttons have configurable hotkeys.
*   upgrades give you passive abilities.
*   and ranged attacks too. they have ATK multipliers, so they get deadlier each version.
*   the Deserialize and Exploit abilities are pretty cool. Just sayin'.
*   fixed a couple engine quirks.
*   fix and tweaked the view model heavily.
*   support map rectangle objects (GID -1). great for triggers over large areas!
*   animations for player, ice and virus crashes.
*   when you crash (health drops to 0) you crash. A nice screen shows and you can restart the level.
*   delayed event posting - wow how handy is this!
*   give upgrades via the @upgrade map object property

8 days ago by wesley (fcebf38): handle the info screen tabs: they can exist in multiple states, and clicking them swaps out the current state instead of pushing more onto the stack. win!

9 days ago by wesley (72094ab): create a UxTabButton that stays clicked, and unselects others in the same group if clicked.

action
------

using a sarcastic terminal:

![using a sarcastic terminal](/assets/alive/devlog/alive-20130721-terminal.png)

a preview of the new tileset:

![a preview of the new tileset](/assets/alive/devlog/alive-20130721-tiles.png)

