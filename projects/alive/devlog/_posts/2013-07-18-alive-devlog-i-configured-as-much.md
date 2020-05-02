---
date: 2013-07-18
layout: changelog
project: Alive
title: "Devlog: I configured as much"
description: ""
category: 
tags: []
---

This post is brought to you by metal.

Moved the story data into a Config like file, we can have nested sections. It proves to show how much neater it all looks!

Notably I got line-of-sight working with the fog. It was an exciting moment.

Old animations config:

    animations = {
        # flat small blue terminal
        41: {
                'frames': [41, 42],
                'fps': 0.2,
                'loop': -1,
                },
        # flat large blue terminal
        43: {
                'frames': [43, 44],
                'fps': 0.3,
                'loop': -1,
                },
    

New configuration:

    [ animations ]
    
        [[ flat small blue terminal ]]
        gid = 41
        frames = 41, 42
        fps = 0.2
        loop = -1
    
        [[ flat large blue terminal ]]
        gid = 43
        frames = 43, 44
        fps = 0.3
        loop = -1
    

There is a new main screen

![menu screen](alive-20130618-menu.png)

Terminal views are now full screen

![terminal screen](alive-20130618-terminal.png)

The dialogue system was reworked, it is now as smooth as silk. You can even skip transition effects and dialogues, something that bothered me before.

