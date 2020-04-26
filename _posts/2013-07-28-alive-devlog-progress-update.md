---
date: 2013-07-28
layout: changelog
project: Alive
title: "Devlog: Progress Update"
description: ""
category: 
tags: []
---

The first milestone now has a name: Y.T, after the streetwise fifteen-year old girl in Snow Crash.

**Completed**

*   blockable walls and map doodads.
*   field of vision.
*   various enemy's to combat.
*   8-bit love.
*   a melee combat system.

**in development**

*   ten levels of digital adventure.
*   a ranged combat system.
*   upgradable character abilities.
*   tracked module music.
*   a nicely packaged release for multiple platforms.

**Some notable changes**

1.  Busy on a branch to rework the Object interactions, these are the things that allow you to trigger other objects on the map, and show story dialogues. The changes allow for delayed interactions, and provide a cleaner command list IMO. See "Object Interactions" under the Dev page.
    
2.  (23610a2): center the viewport around the player if it is out of scope
    
3.  (acc5549): level 1 got servers and (2824700): server tiles! ![server](/assets/alive/devlog/alive-20130628-server.gif)
    
4.  (fcfa642): Ctrl+Function keys for debug events
    
5.  (15f0f09): created draw_animations_cheatsheet() ^F2 to save a png of defined animations
    
6.  (d791372): update block matrix on character movement for los (line of sight)
    
7.  (00ae644): pep8 compliance :D
    
8.  (ecd70f7): real viewport handling for larger map sizes
