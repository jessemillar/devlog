---
layout: post
title: "Week 7 Almost to MVP!"
author: "Jesse Millar"
published: false
---

It's been three weeks since my last post. In the interest of full disclosure, I've had enough content for a new post for the last two weeks. I put off writing this installment because it was just too darn tempting to keep pushing because I'm THIS CLOSE to a working MVP. I've decided it's finally time to publish a new post even though the MVP isn't quite ready. Hopefully there'll be a demo next week!

![*The Staff of Lewis* Week 7 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-7-overview.gif)

Recent progress:
1. Added a `Tombstone` `Skelly` spawner because there needs to be a mini boss for the first level and a tombstone that spawns skeletons was "easier" to implement, feels cool, and helps set the mood of the game
    - As part of that, I drew up a sweet (but rough) spawn animation that I look forward to polishing
1. Enemies notice you when you get close enough
    - You can see the "I noticed you" exclamation marks in the GIF above
1. Cleaning up stack collision checking
    - Makes things more predictable and clean code makes me happy
1. Skellies throw diagonally now
    - Thankfully they don't have perfect aim (I programmatically calculate an innacuracy rate for each `Skelly`)
1. Player stamina (this is probably the biggest change and the most game-like thing I've added recently)!
    - Can't attack when stamina is low
    - There's an indicator in the `Healthbar` and a sweat icon over the player when their stamina is low
1. Loot drop tables
    - I also added in a `Milk` `Collectible` that restores stamina
1. Shaking `Healthbar` when health is low
    - Really helps the player FEEL that they're in trouble
1. Better grass color
    - Your eyes don't bleed when you look at the grass anymore!
1. Added pillars
    - Just for some visual flair
1. Cleaner collision filtering code
1. Made a configuration that makes object immovable
    - I made a lot of changes this week that push things towards more of a configuration-based setup where I don't need custom code for each entity

Next goals:
1. Start building the actual first level
1. Figure out starting dialogue for the first level
1. Find a way to lock framerate or perform calculations that include `dt` (delta time)
    - On some machines (specifically Macs) there is an issue where the game runs too quickly because the FPS isn't locked and I calculate physics based on frame rendering instead of time passing
1. Add a pickup that restores health
1. Start adding more sound effects and music

<iframe src="https://open.spotify.com/embed/track/2XPc8gL9PwxGURQFcFaDJR" width="300" height="380" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>