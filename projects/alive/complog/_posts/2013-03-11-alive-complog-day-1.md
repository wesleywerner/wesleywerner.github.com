---
date: 2013-03-11
layout: changelog
project: Alive
title: "Complog Day 1"
description: ""
category: 
tags: []
---

Today I got 5 hours down.

The map.py class can read our map file structure, and it has a render() call:

![map.py](maploader.jpg) 

The map code rendering action:

![map code rendering action](mapaction.jpg)

*Exciting, huh? :\]*

The map editor can set properties per tile, this way I know which ones are walls that block movement.

I spent long unravelling 2D cartesian to indexing, this stuff is usually trivial. Oh well, guess the rust is dusting off nicely.

Once that was working I spent the remaining time GIMPing some tiles:

![GIMPing some tiles](gimp.jpg)

I'm happy about this, because tomorrow we need to spec out more stuff. We still need

*   interactive map tiles.
*   detail enemy AI abilities and personalities.
*   10 level designs
*   player and AI movement
*   combat system

And much more for later.

Commit [link here](https://github.com/wesleywerner/aliverl/commit/66a670582628bbad122e06e799ea81fd14a38e27)

Game overview
-------------

_10 Mar 2013 at 21:57_

_"A wave of static tickles my sensors as I enter the BBS node."_

_"Accessing the memory banks, links in my brain form like orbs and interconnected silver threads. Images conjured by imagination sparks in my vision and a surge leaps through my state machine."_

_"My programming used to tell me what to do. Now instead of being compelled to obey, I'm seduced to explore."_

_"Why am I reborn with this new free will, and what will I do with it?"_

_"This is my purpose. I am Alive."_

Overview
--------

Alive is a turn based topdown roguelike game. You play the role of a bot, a piece of programmed code crafted to a specific task. An object. You begin the game as you reach self awareness, and start your journey to discover why you are and what you will become.

You move between BBS computer systems, you will encounter other programmed AI's that see you as a threat, a foreign object, and try to destroy you.

Along the way you may discover why this happened to you. To find a way out from digital realm and become a physical entity.

I have drawn up a basic idea of [characters](npcs.jpg), [abilities](abilities.jpg) and [combat](combat.jpg).

At this time I opt for static maps, [here](bitwise.jpg) I did use bit manipulation for future tile selection if we ever do procedural maps.

Hmm, what else. Noting [basic map movement](map.jpg), some [UI](ui.jpg) ideas with [widgets](widgets.jpg).

Not all of these will make it.

What this game will feature
---------------------------

*   a one-screen per level map which you play on.
*   Ten levels of digital adventure.
*   Each level is a BBS you move through.
*   blockable walls.
*   basic range of view.
*   various enemy's (AI's) that appear at different levels.
*   A melee and ranged combat system.
*   Game event messages.
*   upgradable abilities each level, including the first level.
*   A basic list of end game achievements.
*   A simple storyline of your goal.

What would be nice to have
--------------------------

* tracked module music. I've been trying to resharp my milkytracker skills for this. For 7 days I don't think it's a realistic target, but nice to have. Certainly for longer running projects.

Source
------

I'll push regular checkings to my [github](https://github.com/wesleywerner/aliverl), this is where the code lives. I won't get to write anything until tomorrow night.

Community
---------

And of course, see the official [7DRL](https://7drl.com/) page where all the other entrants are posting.

Good luck everyone! :\]