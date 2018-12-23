---
layout: post
title: "Week 4 Holy Progress, Batman!"
author: "Jesse Millar"
published: true
---

Whew! This week had a lot of progress! Most notably, Lewis is now a fully playable character with animations, kicks, and bombs that explode (with a hand-drawn explosion animation), create jelly giblets, and shake the camera. Also, healthbars are a thing and they look pretty darn sexy if I do say so myself. Take a gander!

![*The Staff of Lewis* Week 4 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-4-overview.gif)

This week's spoils:
1. HEALTHBARS
    - Most of this week was spent on health bars. They wound up being more complicated than I thought they'd be largely because I discovered that I wanted to reorganize my codebase to make creating them easier. Things are MUCH more organized now and I'm quite happy about that.
1. Better screen resolution.
    - Before, the game ran at a 200x150 pixel resolution. Now I'm using a 256x160 resolution which makes things a bit more widescreen and actually fits my 8x8 pixel tiles evenly on screen. I refactored some of my healthbar code to be able to dynamically handle different screen resolutions if I decide to change screen sizes again in the future (or if I eventually port the game to mobile and need to support even more screen sizes).
1. Support for fullscreen and window resizing.
    - Makes the whole thing feel more professional.
1. Multiple attack types.
    - There's now a check that runs whenever you hit the attack button. If there's an enemy within punching distance, your character punches. If there's no close enemy, your character makes a ranged attack. It still needs some tweaking, but it feels pretty good on the whole.
1. Slower gameplay.
    - On the surface, that sounds like a bad thing, but it's really not. I fiddled with my physics engine to make gravity and friction take longer to affect things and it makes the game feel more approachable. Things were just too chaotic before.
1. Fixed a large number of bugs.
    - There were a lot of issues with how bounding boxes were handled. I had the coordinate system flipped in a weird way and that caused issues when I was spawning invisible bounding boxes for bomb explosions. Found the issues and squashed 'em.
1. Documentation.
    - I've been making a concerted effort to riddle my code with comments and `README.md` files so future me isn't confused by how past me coded things. Feels good.

Plans for this next week:
1. Make skellies a bit more dangerous.
    - I want them to be able to throw bones diagonally. They're just not enough of a threat as things stand currently.
1. Build a real test level.
    - I want the level to be able to scroll and spawn enemies in designated places and flash "GO!" when it's time to move to the next section. I'll need to build camera following logic to make that happen. I'm also gonna fiddle with using Tiled to designate spawn spots.
1. A "game over" screen.
    - Still don't have a way to restart a level after you die.
1. Make enemies smart enough to switch targets.
    - Especially if their current target dies. Right now, if the player they're tracking dies, they just stick to the spot where the person died.
1. More art.
    - I'm starting to draw portraits for each of the playable characters so I can make a character select screen. Wanna make more progress on that.

Let's see how this Christmas break goes! It's been a productive one so far!