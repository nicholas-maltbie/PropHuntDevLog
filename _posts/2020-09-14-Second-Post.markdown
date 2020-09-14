---
layout: post
title:  "Week 2"
date:   2020-09-14 00:45:00 -0000
categories: update
comments: true
---

This is the second post of the development log

# Progress

There were quite a few changes this week. Most of the project is trying to get the basics up and running. I'm attempting to get a testing framework up and running. Previous post I was talking about this topic and had a few updates.

Within the last week, the following PRS were finally added to the project:
* [Automated Github Builds Actions](https://github.com/nicholas-maltbie/PropHunt/pull/64)
* [Basic Testing Framework](https://github.com/nicholas-maltbie/PropHunt/pull/54)
* [Build Path for Github Builds](https://github.com/nicholas-maltbie/PropHunt/pull/72)
* [Adding Dotnet Format to Project Workflow](https://github.com/nicholas-maltbie/PropHunt/pull/74)
* [Adding Code Coverage to Unity Tests](https://github.com/nicholas-maltbie/PropHunt/pull/71)
* [Client Game Hosting Patch](https://github.com/nicholas-maltbie/PropHunt/pull/77)
* [KCC Follow Ground](https://github.com/nicholas-maltbie/PropHunt/pull/52)

And one PR is queued up about to be finished
* [Unity Upgrade 2020.1.5f1](https://github.com/nicholas-maltbie/PropHunt/pull/78)

These added functions are added to achieve a few main goals
1. Create executable versions of the project with each major update
2. Execute tests to ensure quality of code
3. Path or fix features from previous updates

These goals have been great so far. I'm really liking the progress. I may have to tone back some of my work to get a bit more homework for my courses done but that is besides the topic. I have enjoyed learning a lot more about ECS and getting it to work with the [Unity TestRunner](https://docs.unity3d.com/2017.4/Documentation/Manual/testing-editortestsrunner.html). 

# Future Goals
The current PR being worked on is an update of unity to version 2020.1.5f1. This is an upgrade prompted to me from a post on Unity's forums concerning the nature of preview packages and getting patches and bugfixes with new updates of unity. The major change in this patch is that the unity netcode package updated to [version 0.3.0](https://docs.unity3d.com/Packages/com.unity.netcode@0.3/changelog/CHANGELOG.html). These were quite extensive changes that required me to essentially update all the interactions with network features within the project. Was not a fun task but I learned a lot more about netcode in the process.

The next major set of gaols from the original milestones are
1. Finishing Kinematic Character Controller (KCC) functionality
2. Adding integration (playmdoe) testing and documenting how to add future tests
3. Tweaks and fixes to build pipeline
4. Properly updating documentation for coding style

# Going Forward
I will be working on those goals in some order. I like working with the KCC the most as it's a fun interactive component that can create great visuals. I will attempt to get playmdoe testing working and better document the existing testing and style framework for the project.

There are a few more fixes to the build pipeline but they will have to wait until after I confirm the update to unity version 2020.1.5f1 works as expected.

Overall the project is going well and I hope to have this set of milestones done within the next few weeks. Once all of these basic features have been implemented, I can get to work on more of the fun aspects of the game, transforming into objects and moving around a dynamic scene. From there I can start some rapid prototyping of the game, post it on forums for feedback, support, and advice from others, and see how other people react to the project in general.
