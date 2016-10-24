---
layout: default
title: {{ site.name }}
---

### Syllabus for 2016/2017 school year

Meetings will happen after school in the computer lab on Mondays, starting at around 3:30 (giving you some time to decompress after the school day) and lasting until roughly 5:30. If you need to leave earlier, because a parent comes early, or you're worn out from a long day, or just have mounds of homework, that's perfectly fine.

At each meeting, we'll start with a new programming concept, and an old-school video game that uses it. I'll show you how to use the week's concept in JavaScript, then we'll take a short break before splitting into small groups. Groups can start to implement the feature into our game (two groups working on the same thing is fine), or do related gamework such as making artwork for characters and cut scenes, or writing storylines and dialog.

At the end of each meeting, we'll discuss the work on the game so far, including any new ideas or direction for the game that you have. Lastly, I'll send myself any new code or art changes that need to be merged into the project, and then finish with a "Geek of the week" pop-culture trinket that can be anything from a reference to a 1970s anime show, video game bugs, or maybe something from classic hacker lore.

That night, I'll send out an email to your parents talking about our progress, and a link to and more detailed description of a "Brainiac deep dive" that budding software engineers can study to improve their street cred, glance at briefly and say "man, that's crazy", or ignore entirely.

Here is a (currently incomplete) general outline for each meeting, followed by more detailed descriptions:

| Date | Topic | Description | 
|:-----|:------|:------------|
| Every meeting | Art, story, plot | Talk about your vision for the game, draw stuff, write plot, dialog, character backstories |
| [November  7](#week01) | DOM, canvas, JavaScript | Intro to HTML5 canvases and animation concepts, decide what type of game we want, learn about Github |
| [November 14](#week02) | Conway's Game of Life | List/Object handling, drawing basic shapes, iterating |
| [November 21](#week03) | Pong to Breakout | requestAnimationFrame, collision detection, event handling |
| [November 28](#week04) | Prince of Persia | Rotoscoping! Discuss turning filmed actions into character graphics |
| [December  5](#week05) | Tetris | Context transforms, color, random numbers |
| [December 12](#week06) | Asteroids to Flappy Bird | Physics!, irregular shapes and random levels, discuss speaking at Stir Trek |
|  December 19           | Winter Break | Throughout winter break, I'll be keeping |
|  December 26           | Winter Break | in touch through email, and looking over |
|  January   2           | Winter Break | any new code, art, or story submissions. |
| [January   9](#week07) | Early project demo | Show parents our progress so far |
|  January  16           | Martin Luther King Jr. Day |  |
| [January  23](#week08) | Pacman revisited | AI players, nearest neighbor, goals, sprites, function prototypes |
| [January  30](#week09) | Zork, The Choosatron | Inventory, saving game state, database concepts |
| [February  6](#week10) | Chatroom | Client/server, websockets, Node.js |
| [February 13](#week11) | Chess | Multiplayer! Using websockets for game actions |
|  February 20           | Presidents Day |  |
| [February 27](#week12) | ??? | I'll add more as we go. |
| [March     6](#week13) |  |  |
| [March    13](#week14) |  |  |
| [March    20](#week15) |  |  |
|  March    27           | Record Day |  |
| [April     3](#week16) |  |  |
| [April    10](#week17) |  |  |
|  April    17           | Spring Break |  |
| [April    24](#week18) |  |  |
| [May       1](#week19) |  |  |
| [May       8](#week20) | Final plans | Finish project, schedule demo for all of CA, discuss speaking at Code Mash in January |

### <a name="week01"> Week 1, November 7

The first week I'll demo some of what's possible with programming in JavaScript. I'll draw and animate a Pacman character using no other tool than a web browser. I'll go very fast, because there is a lot to show, but you don't need to worry about memorizing anything just yet. This will be an introduction to the types of things that are possible with programming in JavaScript. As we progress through building the game, you'll learn one piece at a time in more detail.

We'll also discuss what type of game we want to build. _You_ will lead designing the game, and I will help you learn to program so you can build it. You will decide the plot, the type (I suggest a 2D sidescroller or old-school Zelda-like adventure game, because those should be achievable in one school year, and they both line up fairly well with the concepts I plan to teach.)

* Geek of the week: The Pacman ghost pass-through bug
* Brainiac deep dive: [Solving job interview questions in different languages](http://curtisautery.appspot.com/5865619656278016).

### <a name="week02"> Week 2, November 14

This week we'll look at the Finite Automata game "Life", designed by the mathematician John Conway, and an implementation of it in JavaScript. The game shows the birth and death of square "cells" based on how many live cells surrounded it on the previous turn.

Implementing Life teaches us how to handle objects, how to draw a basic shape, and how to pass variables to a generic "function" that will draw a given shape where we want it on the screen. It will also teach us about handling lists of things, such as the two dimensional "array" that we'll need to check to see what cells are on or off.

* Geek of the week: From Superfriends to Ultimen
* Brainiac deep dive: [Life in APL](https://dfns.dyalog.com/n_life.htm). This is an implementation of Conway's Game of Life in the obscure and very mathematical looking language "APL".

### <a name="week03"> Week 3, November 21

This week we will learn from the old school games Pong and Breakout how to react to user actions such as moving the mouse or pressing keys (arrow keys, in this case) by using event listeners. We will also learn some early methods of controlling how many game "frames" are painted each second, and the better modern approach using "animation frames".

* Geek of the week: The Konami Code, and ID Software's IDCLIP
* Brainiac deep dive: [Solving Sudoku with Java](http://cautery.blogspot.com/2010/09/building-java-applet-sudoku-bot.html).

### <a name="week04"> Week 4, November 28

This week we'll learn the history of rotoscoping from the 1989 Apple // game "Prince of Persia", the first game to use live video of a person as the basis for animations. Their technique was weird, because of the limited tools available, and modern tools make the process much simpler now.

We'll also start deciding who is going to be our camera operator, what types of human actions we want in the game, ask for volunteers to be actors, and get parents to signoff on the process. The technical process will involve filming an action, for example running and changing direction, identify where all the limbs are in each frame of the action, and join the limb information with character art. The final in-game result will be slightly more detailed than Mario, but actions will appear more natural and fluid... because they were natural and fluid motions made by humans.

If we end up speaking about the project at a local convention, I'd like to show some of this process, which would include raw video clips of the pre-rotoscoped actions, and possibly even a "meta" clip where a second camera is watching the whole process... hence I'm being especially sensitive to whether club members know everything involved, have volunteered, and that there aren't any misgivings about the process from parents or school staff.

* Geek of the week: 7 Zark 7
* Brainiac deep dive: [Animated prime number machine](http://cautery.blogspot.com/2012/05/animated-prime-number-machine.html).

### <a name="week05"> Week 5, December 5

This week we will learn from the game Tetris how to use "affine transformations" to draw a fixed shape at different positions, rotations, and sizes. We will talk about handling color, from different colorspaces, to transparency and mixing colors, and we'll crack open the drawing tablet and the Sketchbook program, and see if drawing that way clicks with anyone.

* Geek of the week: The Enigma Machine
* Brainiac deep dive: [Fun with command-line Perl](http://curtisquarterly.blogspot.com/2005/05/perl-tutorial.html)

### <a name="week06"> Week 6, December 12

This week we will learn from Asteroids, Joust, and Flappy Bird how to incorporate simple physics into our game. In Asteroids, your ship has inertia, so it slowly speeds up as you apply thrust, continues in the same direction until force (from an impact, or from thrust in a different direction) changes its vector. In Joust and Flappy Bird, gravity pulls us down, and flapping wings applies force to overcome gravity. We'll talk about various ways to implement those effects in-game.

The December/January timeframe is when the local tech convention "Stir Trek" starts taking submissions for talks, and the conference itself happens sometime in April or May. If we feel by this time that we'll have a semi-functional game by April, I'd like for us to consider registering to give a talk at the conference about the club, learning to program, and the game itself. If we do that, the talk would consist of me giving a brief overview of my vision for the club, and then hand the mic off to one of you to give the main body of the presentation, while I run the computer showing our presentation slides, or whatever our media is. We will present the project to the school at some point close to the end of the year, which could function as a dress rehearsal for speaking at a conference.

If any of the club members have public speaking chops, or would like to try it out, we can practice with some AV equipment throughout the year at a suitable location. As with the Rotoscoping video permissions above, I want to make very sure at this point that the school and the parents of any volunteers are on board with this before making a formal submission to Stir Trek's call for speakers.

* Geek of the week: Simon/Merlin
* Brainiac deep dive: [Using an abacus to calculate in Base 18](http://cautery.blogspot.com/2013/04/base-eighteen-on-chinese-abacus.html)

### <a name="week07"> Week 7, January 9

### <a name="week08"> Week 8, January 23

### <a name="week09"> Week 9, January 30

### <a name="week10"> Week 10, February 6

### <a name="week11"> Week 11, February 13

### <a name="week12"> Week 12, February 27

### <a name="week13"> Week 13, March 6

### <a name="week14"> Week 14, March 13

### <a name="week15"> Week 15, March 20

### <a name="week16"> Week 16, April 3

### <a name="week17"> Week 17, April 10

### <a name="week18"> Week 18, April 24

### <a name="week19"> Week 19, May 1

### <a name="week20"> Week 20, May 8

More soon!