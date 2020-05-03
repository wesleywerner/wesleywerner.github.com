---
layout: project
title: "Lua Star"
description: "A pure Lua A* path-finding library."
thumb: /projects/luastar/thumb.jpg
links: ["GitHub", "https://github.com/wesleywerner/lua-star"]
status: stable
---

A tiny Lua 5.x compatible library to easily add A* path finding to any project. 

The repository includes an example created in [LÖVE](https://love2d.org/), unit tests and a performance profiler.

The path finding is super fast, averaging 16 milliseconds to find a path on a map with 9 million locations, with about 65% open space.