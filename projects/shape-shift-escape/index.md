---
layout: project
title: "Shape-Shift Escape"
description: "You are a changeling monster locked up in a secret lab. You must escape before they test you to death!"
thumb: /projects/shape-shift-escape/thumb.png
featured: true
featuredimage: /projects/shape-shift-escape/featured.png
links: ["LD Entry", "http://ludumdare.com/compo/ludum-dare-33/?action=preview&uid=26303", "GNU / Linux", "http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-postcomp-linux.tar.gz", "Win", "http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-win32.zip"]
status: stable
---

**Ludum Dare 33 Entry, 2015**

This is a point-and-click adventure game created using the [SLUDGE game engine](https://opensludge.github.io/). Sound effects were generated with SFXR, Pixel art by myself.

![](/projects/shape-shift-escape/screenshot.png)

* [Submission SLUDGE source](http://keyboardmonkey.co.za/ld33/LD33%20You%20are%20the%20monster-source.zip)
* [Submission GNU / Linux](http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-linux.tar.gz)
* [Submission Windows](http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-win32.zip)

I released a post-compo version that fixed and added a few things.

* [Post comp GNU / Linux](http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-postcomp-linux.tar.gz)
* [Post comp Win](http://keyboardmonkey.co.za/ld33/LD33-keyboardmonkey-youarethemonster-postcomp-win32.zip)

Post Comp Fixes

* The coffee cup falls sideways when spilled, and the security guard no longer says "hands off" when you try to take it (even when he was knocked out by the gas).
* Fixed the shape-shift animation glitch.
* Prevent guards and scientists from saying something random when there are words on screen.
* Lower music volume. It overpowered the game sounds.
* Loop game music when it ends, instead of restarting the music when re-entering the hallway.
* Better placement of the lab exit hotspot.
* After the scientist tells you not to touch the knockout gas, resume his working animation.
* Restart the game on fail, instead of exiting.

Additions

* Draw pictures on the security room tv's. Add descriptions for the tvâ€™s and bulletin board.
* Replace the key with a security pass.
* Add the level exit as a new room. The door requires a security pass.
