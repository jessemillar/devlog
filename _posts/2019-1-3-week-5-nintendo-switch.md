---
layout: post
title: "Week 5 Nintendo Switch"
author: "Jesse Millar"
published: true
---

Alright. Full disclosure time. This last week and a half or so hasn't been super productive for *The Staff of Lewis*. My parents surprised my wife and me with Nintendo Switches for Christmas and they've done a fantastic job of distracting me from pretty much anything that's not [*Pokémon: Let's Go, Eevee!*](https://twitter.com/jessemillar/status/1080642036221411329) or *Just Dance 2019*. Thankfully, I did make some progress, it's just not amazingly exciting progress.

![*The Staff of Lewis* Week 5 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-5-overview.gif)

Christmas break accomplishments:
1. Build system with [love-release](https://github.com/MisterDA/love-release)
    - I've got a [custom Docker image](https://github.com/jessemillar/arch-love-release) built and tied with [CircleCI](https://circleci.com/) that automatically builds and pushes LÖVE binaries for different operating systems whenever I push a commit to my `master` branch. It took longer than I would have liked, but it'll definitely be worth it in the long run and I can use it for future games too!
1. Almost have a working character select screen
    - I did custom pixel art for character portraits on the character select screen and reorganized player setup code to allow for dynamic character selection. Getting close but there's still a "null pointer" error.

Next week's plans:
1. Finish character select screen
    - I still need to figure out how to call constructor methods based on which character is selected to fix that blue screen error in the GIF above.
    - I also want to improve the pixel art and the way it's presented on screen. It's a bit too bland currently and there's no indicator of which character is currently selected by which player.
1. Make enemies more fun to fight
1. Scrolling camera with scrolling level