---
layout: post
title:  "First Post"
date:   2020-09-08 12:47:00 -0400
categories: update
---

This is the first post of the development log.

The game has not had too much progress as of now. This blog will also be updated with the current development goals on some other page in the future. In addition there will be weekly update posts.

# Goals
Version 0.1.0 goals:
1. [Automated Build Pipeline](https://github.com/nicholas-maltbie/PropHunt/milestone/5)
    * Pipeline to generate server and client versions of software
    * Should be done automatically as part of release cycles
2. [Documentation and Style Guidelines + Enforcement](https://github.com/nicholas-maltbie/PropHunt/milestone/7)
    * Enforcement of consistent style either through changing code, raising errors, or both
3. [Testing Framework](https://github.com/nicholas-maltbie/PropHunt/milestone/4)
    * Automated testing framework with code coverage
    * Integration and Unit testing framework for all user written code
    * Avoid generated code
4. [Kinematic Character Controller](https://github.com/nicholas-maltbie/PropHunt/milestone/1)
    * Character controller that uses Kinematic physics to move the character irrelevant of world physics
    * Still stay without bounds of world
    * Allow for non human control of KCC
    * Support these features
      * Fall due to gravity
      * By stopped by dynamic or moving colliders (no walking through walls)
      * Move with objects that player is standing on (rotational movement too)
      * Walk up/down slopes
      * Walk up/down stairs
      * Push objects in virtual environment
5. [Main Menu and UI](https://github.com/nicholas-maltbie/PropHunt/milestone/3)
    * Main menu to connect to a game
    * Menu to leave a game when connected
6. [Basic Network Flow](https://github.com/nicholas-maltbie/PropHunt/milestone/2)
    * Let players join and leave a game (and reconnect to a game they leave)

# Tracking
All of these goals are tracked through [milestones](https://github.com/nicholas-maltbie/PropHunt/milestones) and issues on GitHub

# Progress

All of these goals have been partially or fully completed in the current state of development. 

Here are some samples of progress

## Pushing Cubes
Player pushing around some physics objects (cubes) in a test scene
![Player pushing cube object in a test scene](https://drive.google.com/uc?export=view&id=1x6J4Munto54rBrfuJdZ6Tb12Y10_H-84)

## Disconnecting
Example of players disconnecting and reconnecting to a server
![Using the Unity UI to disconnect and reconnect a player to the game](https://drive.google.com/uc?export=view&id=1Pcq0zZmWFOrZ0axH7po5128RF8CkfnUC)

## Kinematic Character Controller Input
Example of a player moving through an environment using a Kinematic collider object as the character avatar
![Moving through environment as capsule collider](https://drive.google.com/uc?export=view&id=19KHRFQ5WI72MIlM6k773cXjRowxOI3q8)

## Testing Progress
There is also an [in progress PR #54](https://github.com/nicholas-maltbie/PropHunt/pull/54) for testing (just unit testing for now) and generating a code coverage report. This can be extended to include integration testing (called play mode testing) in the future as well. 

Picture of code coverage report
![Code coverage report html page](https://drive.google.com/uc?export=view&id=1xr18qkRAPjmDkkmlDOHdhj2Loyl_roxv)

Picture of edit mode testing panel listing created tests
![Testing panel and available unit tests for Camera Follower System](https://drive.google.com/uc?export=view&id=1XJS79iLnyJE0r9qr0Q4jzmLAbrJBog3L)

Many more features currently have been completed by now as well. Look at all the milestones for more information.
