---
layout: post
title:  "Week 3 : Unexpected Update"
date:   2020-09-21 16:11:00 -0000
categories: update
comments: true
---

This is the third post of the development log.

# Updates (literally)

This week did not have as much of progress. Originally it was planned to work on the Kinematic Character controller and make a test scene but that got interrupted by another unity update. This time the netcode version 0.4.0 (There is no new documentation page as of now). The big changes for this update are that it fixed a few bugs in the client server bootstrap, and enforce the subscene workflow.

The subscene workflow was the big change that broke all the existing code. The current build workflow no longer works and it introduced an odd error where client side objects that controlled by the server are duplicated when the client rejoins. I found a roundabout solution to this problem that I describe on the unity forums in [this post](https://forum.unity.com/threads/netcode-and-subscenes-question.972954/).

This debugging and fixing the build workflow are currently in [PR #83](https://github.com/nicholas-maltbie/PropHunt/pull/83) for the project. This is the current progress for this week along with a few documentation and refactoring changes.

# Going Forward

The immediate goals for next week are to:
* Improving the kinematic character controller to move out of overlapping objects
* Making a test scene with multiple environmental attributes for the KCC to interact with
* Making a performance test scene with hundreds to thousands of KCC's moving around to test the system for where the performance bottlenecks exist. 
* Finishing implementation of play mode testing. (this one serves as integration testing of the project).

A farther off future goal are to recreate the automated build pipeline (as it is disabled now), and update the documentation to describe how to create playmode and editmode tests. Maybe some enforcement for minimum code coverage for these features and adding them back into the checklist for new code.
