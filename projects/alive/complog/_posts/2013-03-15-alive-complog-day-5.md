---
date: 2013-03-15
layout: changelog
project: Alive
title: "Complog Day 5"
description: ""
category: 
tags: []
---

Today we added support for once off triggers, messages, and dynamic property giving.

Triggers allow us to do some crafty things with the game levels. We can close and open doors, turn terminal computers on to be used, that kind of thing.

These actions are set when using the Tiled map editor.

![caps](tile5.png) 

We have capacitor tiles which can pop when the player throws a switch, uses a terminal computer, or walks over a plate trigger.

The file ai.def defines all NPC stats, like health, attack, and so forth.

Some more map additions, and collisions are handled between npc's and player.

Oh and characters now heal over time (both the player and artificial AI's).

### Object Interactions

Give map objects these properties to interact with the game. The action names only match the start, you can add any descriptive words after the name (you can't have two actions with the same name). You may also append any action name with the word 'once' for that effect.

*   message=text: print an in-game message.
    
*   fingers=name: action the named object. It's actions will process, except for other finger actions. You can finger multiple object with 'finger 1', 'finger that enemy', 'finger door'. Object that share the same name will all be fingered too.
    
*   on\_finger=action: where action is one of:
    
    *   give=value: give this object a new property This simulates a terminal that has to be fingered for it to work later, like a power switch or an unlock.
    *   transmute=id\[,id..\]: change this object tile to another. A comma list of id's will rotate between each. This simulates open/closing doors.
*   dialog=name: show the dialog text by name as defined in dialogs.def
    

Examples: A wall switch has these actions: + fingers: "secret\_door" + message: A secret door opens change the tile to a non blockable one, and tell the player about it.

    A door has these:
    + on_finger: "transmute=2,3"
    The door will open and close 9rotate it's tile id) between 2 and 3.
    