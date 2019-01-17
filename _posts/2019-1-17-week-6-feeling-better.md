---
layout: post
title: "Week 6 Feeling Better"
author: "Jesse Millar"
published: true
---

Aw, heck. I didn't realize it'd been two whole weeks since my last post. My bad. At least I have a lot to show for the time!

![*The Staff of Lewis* Week 6 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-6-overview.gif)

This week:
1. Working character select screen
    - Allows P1 to play as either playable character or for a second player to jump in and play as whoever P1 isn't playing as.
    - It should be modular enough to allow the addition of more playable characters without having to redo everything.
1. Ripped out outline shader
    - I have some currently-being-drawn sprites that need outlines only on a portion of the sprite instead of all the way around. I don't foresee myself having outlines drawn through barriers (e.g. a wall in front of your character but you can still "see" your character through the wall via its outline) so it felt like wasted CPU cycles.
1. Fleshed out tilemap graphics
    - I learned more about Tiled terrain setup so now I have grass, dirt, water, and stone that can be drawn with Tiled terrain brushes.
1. Entities can be placed via the tilemap
    - This one took a while but allows me to quickly build levels without hardcoding X and Y coordinates for each entity. There's still some work that needs to be done (X offset is a bit nasty behind the scenes and objects can't currently stack), but I'm pretty happy!
1. Moved from using [`hump.camera`](https://hump.readthedocs.io/en/latest/camera.html) to [`gamera`](https://github.com/kikito/gamera)
    - This move allowed for easier camera movement that follows the player(s) and is constrained to the size of the level.
1. Enemies intelligently select targets now
    - This means that enemies don't infinitely stand over the dead corpse of a player character. They'll pick a new player once they kill their current target.
1. Added small healthbars above enemies
    - This really improves the quality of life of the player because it makes you feel like your attacks actually matter instead of just being soaked up by a mob.
1. Objects are constrained to the visible screen now
    - No more running into the abyss!

Next week:
1. I'm trying to figure out what classifies as a minimum viable product (MVP) so I can start having some people playtest. The problem is that I keep thinking of new features that I want to have in the MVP which is pretty much the opposite of [what an MVP should be](https://www.youtube.com/watch?v=z06QR-tz1_o).
    - There's a chance that I'll add more destructible objects to the first playable level because breaking things feels pretty good.
1. Finish the tombstone skelly spawner
1. Make skellies able to throw diagonally
1. Tweak Lewis to make bombs more fair
    - It feels like he can do too much damage too quickly