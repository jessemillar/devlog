---
layout: post
title: "Week 3 Shaken, Not Stirred"
author: "Jesse Millar"
published: true
---

Lots of personal and work-related things hit the fan this week so I wasn't as productive as I'd have liked. Having gamedev goals has definitely been showing me how much and how little free time I really have.

![*The Staff of Lewis* Week 3 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-3-overview.gif)

What I did:
1. Started work on health bars
    - There's now a health bar in the top-left corner of the screen. It doesn't show the player's health and doesn't have lives or score or anything yet, but it's there!
1. Implemented [hump camera](https://hump.readthedocs.io/en/latest/camera.html) so the camera can rove across the level's tilemap
    - It was a bit of a struggle to get screen shake working with the hump camera. Initially, I tried using a library called [shack](https://github.com/Ulydev/shack) which worked but seemed to shake different parts of the screen in different ways (the health bars in the UI would shake for longer than the players). I ended up implementing my own screen shake with the hump camera based on some snippets in the hump documentation. It works great and now the UI doesn't shake with the rest of the screen!
1. Improved tilemap look
    - Basically, this means the tilemap in my test level looks more polished. You can see the results in the .gif above. This was actually a lot easier than I thought it would be thanks to the [Tiled](https://www.mapeditor.org/) terrain drawing brush. I just had to tell Tiled how to interpret my spritesheet and then it knew exactly how to draw terrain when I dragged my mouse over the tilemap. Nifty!

What I want to do next week:
1. Get multiple attacks working
    - Each player character will have a punch attack and a ranged attack. Both are triggered by the same button which means the game needs to be smart enough detect if a punch would connect and if not do a ranged attack instead.
1. Make Lewis work
    - You can control Lewis now and jump on enemy heads, but you can't attack.
1. Implement a game over state
    - I want a screen that says "game over" and takes you back to the menu if both players die.

I'm pretty excited for Christmas break! Hoping I'll be super motivated when I just have a lot of free time.