---
layout: project
title: "Virulent"
description: "Turn-based tactical game managing a viral outbreak."
thumb: /projects/virulent/thumb.png
links: ["Pico-8 Cart", "/projects/virulent/virulent.p8.png", "Löve Release", "https://github.com/wesleywerner/virulent/releases", "Source", "https://github.com/wesleywerner/virulent", "Play Online", "https://www.lexaloffle.com/bbs/?tid=39153"]
status: stable
---

Virulent is a turn-based tactical game where you are in charge of managing a global viral outbreak, and if you are lucky, save the world.

I dedicate this game to every person who has been separated from their family or loved ones during the tragic corona virus outbreak of 2020. We miss you dearly.

# Screenshots

### command screen
![command screen](/projects/virulent/virulent_1615638100.png)

### region info
![region screen](/projects/virulent/virulent_1615286219.png)

### apply remedy
![remedy screen](/projects/virulent/virulent_1615286107.png)

### radar tracking
![radar tracking screen](/projects/virulent/virulent_1615286081.png)

### turn report
![turn report screen](/projects/virulent/virulent_1615286061.png)

### scores
![score screen](/projects/virulent/virulent_1615285946.png)

### end game world report
![end game world report screen](/projects/virulent/virulent_1615285977.png)

# Get It

The Löve Release is linked above. You need [Löve](https://love2d.org/) to run it.

The Pico-8 version is available as a cartridge, also linked above and shown below. You need a copy of the Pico-8 fantasy console to load this cartridge.

![pico-8 cart](/projects/virulent/virulent.p8.png)

# Game Instructions

Virulent is a turn-based game where you use action points to manage a viral outbreak on earth. The story is that the earth is hit by asteroids carrying a deadly virus, your task is to launch missiles to prevent any more infections, while administering remedies to infected countries and cure them.

### Mute

Press `control` + `m` to mute/unmute audio.

### Full screen

Press `alt` + `return` to toggle full screen.

### Controls

To highlight a country, choose a remedy or select an asteroid:

`up`, `down`, `left`, `right` arrow keys.

### Actions

To open country details or press a toolbar button:

Press the `X` key.

### Shortcut key

Press the `Z` key.

On all screens you can use the `Z` key as a shortcut instead of using the toolbar.

- On the Regional screen, it opens the remedy screen if a remedy can be applied.
- On the Remedy screen, it applies the selected remedy.
- On the Radar screen, it launches a missile.
- On the Command screen, it ends the turn (only when no more actions can be performed).

### The Toolbar

The toolbar is located at the bottom of the screen. Use the arrow keys to highlight a button, and `X` to press it.

On the Command Station screen, press the `down` key to focus the toolbar at the bottom. To return to country selection, press the `up` key.

Instructions are in-game. Choose the Help toolbar icon to read them.

# History

Virulent is a remake of an Atari game called "Epidemic!" by Steven Faber (1982).

I started the project in July 2020 for the [Pico-8](https://www.lexaloffle.com/pico-8.php) fantasy console. It took 4 weekends to complete. I referenced the [original game manual](http://www.atarimania.com/game-atari-400-800-xl-xe-epidemic_1859.html) to derive the game mechanics. I updated the world data to reflect modern country names and statistics, and added three new countries - Madagascar, Southeast Asia and South Africa.

If you would like to play the original game by Steven Faber, you can find the Atari version from [myabandonware.com](https://www.myabandonware.com/game/epidemic-26#Atari%208-bit) and use an emulator like [atari800](https://atari800.github.io). The DOS version is not playable, in my opinion.
