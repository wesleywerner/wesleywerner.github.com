---
date: 2013-03-12
layout: changelog
project: Alive
title: "Complog Day 2"
description: ""
category: 
tags: []
---

Today's changes are for the brain of the map engine. We can move our characters around the map, it is blocked by walls, and there is a neat callback when we run into game objects.

This includes a way to perform actions on some objects, like a switch to open a door. This is defined within the map editor itself, giving great flexibility over the tiles we have.

I battled with drawing the different canvas layers with transparency, the part where clearing the previous spot of an object, before drawing it's new location. Filling the layer with magenta and setting it as our transparency key works okay.

That's all.

![walking into things hurts](collisions.png)

_Edit:_

Using the Tiled map editor, by adding the 'blocks' bit to a tile's properties makes walls in game. The objects layer items will always block a player. They also call back so we known what is happening.

So adding a map object with the property "action_transmute" with a value to the new tile_id. We can test for this on object collision callbacks. Transmorgify! Thus we can open a closed door. Transmute drops away after the first time.

The "action\_finger" allows a tile to point to another tile to action instead, who can transmorg. We use the target's name as the value -- map objects have name & type properties -- Now we open doors with switches.

We can have both actions on the same object, effectively expiring and fingering an accomplice. Chainload a few and instant bridge or flooding.

It becomes a npc (ambush) or item (rewards) spawner.