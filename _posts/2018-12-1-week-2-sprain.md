---
layout: post
title: "Week 2 Sprain"
author: "Jesse Millar"
published: true
---

This week wasn't as productive for *The Staff of Lewis* as I'd hoped it would be. I blame that on the fact that I [sprained my ankle really badly while skateboarding](https://www.instagram.com/p/Bqs7EwTF5Jz/) on Monday. I went to a doctor because my wife and I were convinced that I'd torn something but thankfully the x-ray came back clean. I've been largely couch/bedridden since which has killed a lot of my motivation.

![*The Staff of Lewis* Week 2 Overview GIF]({{site.baseurl}}/images/staff-of-lewis-week-2-overview.gif)

Things I did:
1. Finished making the switch from IntelliJ IDEA to Visual Studio Code for my IDE
1. Made Pablo capable of punching
    - This involved breaking up some of my parent class code so it would be easy to create invisible objects for punch hit boxes (which will be reusable for explosions and doors)
1. Built a system for running an animation once and returning to a default animation
    - I'm using this for the newly-added punch animations (I needed Pablo to return to either his idle or walking animation after a flurry of punches)
1. Fixed four or five drawing bugs
    - There were issues with offset, pivot points, and mirroring
1. Tweaked the physics engine to start to make punches feel better
1. Made local co-op controls work

Next tasks:
1. Not break my other foot
1. Make the outline shader capable of tinting sprites red when objects are punched/damaged
    - There may be an easy way to do this, but I might try actually tweaking the shader code to learn more about shaders
1. Finish making the skelly smarter
    - He currently 
1. Add some attacks to Lewis so local co-op can be playtested
    - He's gonna be able to punch and throw bombs
1. Experiment with button combinations
    - I want a sky pound attack at the very least

I'm trying to be better about my expectations for myself from week to week. While I want this game done by the deadline, I also wanna have a good work/life/hobby balance. Week 1 wasn't very balanced (I worked too much on this project) and week 2 had far too little work done. Gotta be better at using my planner and getting up on time so I can keep hitting goal deadlines!