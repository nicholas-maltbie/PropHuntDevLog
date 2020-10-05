---
layout: post
title:  "Week 5 : Hackathon Among Us"
date:   2020-10-05 00:53:00 -0000
categories: update
comments: true
---

This the fourth post in the development log. I missed last week
but hey, I have a lot to say now.

# Enhancements


## KCC
As far as updates go, the Kinematic Character Controller is nearly complete.
The features of being pushed out of other objects, moving with moving objects on ground, and syncing the player camera between server and client are all up and working now. This is a great achievement and gives the character model a lot of flexibility. 

![Sample movement animation](https://drive.google.com/uc?export=view&id=1waPaxv44uAImOLfxdVxipSz02E-TaNtD)

## Prototype Map
There is also a test stage for moving around the map and adding new content, part of [PR #102](https://github.com/nicholas-maltbie/PropHunt/pull/102)

![Being in a scene with two other players across internet (Canada and US) ](https://drive.google.com/uc?export=view&id=1Zp38wIbpLsErqifKh8Ti8RJ_-n2vBepA)

## Integration Testing

I added integration testing and the only down side so far is that players have to manually create a scene to do tests instead of being able to make virtual scenes through code. It works but cannot be run in an automated pipeline so it may be ignored for now.

## Universal Render Pipeline

I wanted to make the project look better so as part of [PR #100](https://github.com/nicholas-maltbie/PropHunt/pull/100), we added the universal render pipeline to the codebase for shader graphs and other kinds of visual effects and features.

# Perspective

These advancements in the project have taught me a lot about what can be done with the project
and where we can develop from here. I'm really looking forward to these changes
and am hopeful of releasing the initial version of the project and posting it on social media
and forums by the end of October (unofficial goal time). 

I'm learning a lot more about C# and keeping my coding skills up to speed. I'm very happy with this progress and what I've been learning. 

Also I'm blown away by the performance of the project. I'm running into a bit of conflict with managing my graduate work as well but hopefully I will be able to take a break (or work at a reduced rate, maybe only write unit tests) for a week or two while I get caught up with my graduate studies these next few weeks.

# Future Goals

The only goals left for the initial version of the repository are:
1. Full Coverage Unit Testing
  * Documentation on how to make unit tests
  * Enforcement of code coverage
2. Fixing automated build pipeline?
  * Will probably just ignore this for now as it's not necessary
3. Kinematic character controller features
  * The last features to add are walking up and down stairs (and ramps?) smoothly
  * Creating a set of more rigorous test objects in the test scene
  * Addressing some of the follow floor jitter?
    * Solution seems to be to just giving the player a wider room for
      error when standing on vertically moving platforms, horizontally 
      moving platforms do not seem to cause an issue. 
  * Processing movement on a tick basis instead of frame basis to have
    more consistent behaviour.

# Hackathon

![Sample movement animation](https://drive.google.com/uc?export=view&id=18vgUN4-nVSaMfI3QwAm1ctLknWBuL6qx)

As mentioned in the title, me and a few friends made a copy of the repository to start development of a duplicate project reusing a lot of the same code and features to create a clone of the game Among Us. The cloned repo we called Spaceship Murder Time and can be found here [https://github.com/nicholas-maltbie/SpaceshipMurderTime](https://github.com/nicholas-maltbie/SpaceshipMurderTime). 

This added a lot of new features that will be moved to the PropHunt project as well. These features include
* Loading scenes dynamically
* Having a lobby scene and starting a game
* Player models attached to a character
* Cel-shaded graphics
* Commands to change loaded character model (really important for prophunt, less so for among us)

This was a great advancement in the project as we're really happy that the project as been able to develop this way so far. There is no way I would have ever made this much progress with learning netcode communication as quickly if it wasn't for this hackathon and sitting down and coding for 20 hours in a day. I'm really happy I got the chance as I also learned a lot more about URP, some about unity animations, as well as other advancements in the project.

This will probably be developed as its own separate project and just have us copy and port code between the two projects.

I will work on a scene loading system for the PropHunt game as well and it will be a much cleaner and better formatted version that what exists in the PropHunt game so far. I'm happy with all the progress and look forward to what this will achieve in the future.

Project Devpost Submission: [https://devpost.com/software/spaceship-murder-time](https://devpost.com/software/spaceship-murder-time)
