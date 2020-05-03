---
layout: project
title: "MVC Game Design"
description: "A practical guide to design patterns in games."
thumb: /projects/mvc-game-design/thumb.png
links: ["Online Document", "https://engrams.dev/mvc-game-design/"]
status: stable
---

This document details how to implement the MVC design pattern for games. The repository contains a working demo of Same-Game written in Python but this design pattern can be implemented in any language.

By decoupling the View, the Controller and the Model, and using an event manager to communicate between them, we make the code more maintainable, and it allows us to implement other neat controllers like:

- a View for reduced graphics to fit on mobile devices.
- a Controller for touch screens devices.
- Networking.
