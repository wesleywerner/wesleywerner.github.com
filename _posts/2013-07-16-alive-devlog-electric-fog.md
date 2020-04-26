---
date: 2013-07-16
layout: changelog
project: Alive
title: "Devlog: Electric Fog"
description: ""
category: 
tags: []
---

This update is brought to you by git branching, hot drinks and popcorn.

I polished the fog that covers unseen and out-of-range map areas.

![electric fog](/assets/alive/devlog/alive-20130616-gameplay.png)

This was a good rewrite.

*   overlay fog for seen areas and black out unseen areas
*   separate move_player() and move_object(), to handle visible object in range better.
*   fix the running path so relative resource paths work
*   only trigger 'exit' and 'message' actions with direct interaction
*   refactor method names to match PEP8
*   add floating game messages
*   add exit portal animation
*   allow map-level overwrites of character stats

you can now override ai modes and behaviour on a map level for nicer level immersion.

*   resize game window to 600x600 pixels

it now fits onto netbook screens

*   polished the computer terminal screen

![terminal](/assets/alive/devlog/alive-20130616-dialogue.png)

*   add a microchip animated tile
    
*   ai now have movement speeds. can you outrun them...?
    
*   added a list of computer controlled movement behaviours:
    
    *   random: moves in random directions.
    *   magnet: moves towards the player while in sight.
    *   updown: patrols up and down, turning around when blocked.
    *   leftright: patrols left and right, turning around when blocked.
    *   sniffer: follows the player's scent if on the trail.

these can be stacked, so a 'updown, magnet' will patrol and then move toward you if you get too close.

*   update story dialogue texts
    
    *   allow multiple empty lines
    *   supports dialogue color per line by defining a tuple like ((r, g, b), "dialogue line here"). lines that are just strings will display with the default color.
*   you can have 'friend' AI types
    
*   checks collisions for stacked objects including triggers
    
*   cannot close doors if something is blocking the doorway.
    
*   walking into walls and triggering switches counts as a turn.