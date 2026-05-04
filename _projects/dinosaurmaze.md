---
layout: post
title: "Dinosaur Maze"
image: "/assets/projects/DinosaurMaze-thumbnail.png"
excerpt: 🐍 PyGame-based 2D game, where you navigate a maze and avoid a T-rex. Vibe coded with Claude Code in VS.
date: 2026-05-04
---

<figure>
  <img src="/assets/projects/DinosaurMaze1.png" alt="Dinosaur Maze gameplay" width="600">
</figure>

With the creation of this game, I wanted first and foremost to explore the potential of vibe coding using [Claude Code](https://claude.ai/code), Anthropic's AI-powered coding assistant. Secondly, I wanted to make a fun kids game that I like, and hopefully my son too.

If you are curious on the game, please find the source code, game files and description <a href="https://github.com/LaReiter/PLACEHOLDER" target="_blank">on my Github</a>.

Here I will not go into details with the game, but rather the process of game development through collaboration with an AI.

### The game manifest

It all started with some imaginative thinking. I love mazes. My kid, and to some extent myself, love dinosaurs. Can we build a game of mazes and dinosaurs? Definetely. 

I wrote down my thoughts on how I imagined this game, from the visuals to the game mechanics. I wrote down my thoughts in a concise and structured way, that I knew any language model would be able to quickly decipher.

My thoughts - this game manifest - was saved as a .txt file inside a folder that I called **Dinosaur Maze**. Based on this manifest, I knew what this folder would eventually contain, and I began making the proper subfolders for all the graphics.

**Note** My game manifest can also be found <a href="https://github.com/LaReiter/PLACEHOLDER" target="_blank">on my Github</a>.

### The graphics 

I decided I wanted 3 cartoon figures: an adventurous hero, a t-rex and a brachiosaurus. I wanted simple animations: two frames per movement cycle would do. 

Thus I would be needing 6 snapshots of these figures. Two frames for vertical direction (using reflection, we can decide on left/right). Two frames for up movement (with the back of the figure facing the viewer). Two frames for down movement (with the front of the figure facing the viewer).

To generate these figures, I used other large language models (LLMs) with integrated graphics-rendering capability.

To first produce the right prompt for these tools, I had a short conversation with Claude, talking about how I imagined these figures. Among other details, I stressed that each frame should be distinct to fully capture a movement cycle. 

Eventually, Claude produced sufficiently detailed prompts for each figure, that I could then prompt to the graphics-rendering LLMs.

After repeating the prompts and giving some smaller adjustment requests, I was satisfied with the result.

Using the integrated background removal tool to of Photos (windows pre-installed), I was able to obtain transparent background necessary for in-game deployment. 

<figure>
  <img src="/assets/projects/DinosaurMaze2.png" alt="Dinosaur Maze level" width="600">
  <img src="/assets/projects/DinosaurMaze3.png" alt="Dinosaur Maze mechanics" width="600">
</figure>

### The implementation

Through Visual Studio (VS) Code, I navigated to my folder, which now contained the game manifest (readme.txt) along with the finalized graphical items. 

I used Claude Code as a plugin in VS to read the manifest, and search the folder to get an overview. I then asked Claude to make a plan for how to implement this game.

Claude Code came up with a plan, which we adjusted through a conversational back-and-forth.

Once I was satisfied with the plan, I requested that Claude Code wrote a readme.md file, that described everything relevant to the game (e.g. folder content, game mechanics, implementation strategy).

Finally, I asked Claude to execute the plan and Claude responded by producing the required Python files.

The intial result was not perfect. The game didn't look impressive, and there were a couple of issues with the game mechanics.

Through a iterative and conversational process, these things were quickly fixed.

The idea of the game was conceived one early evening. The next evening, the game was done.

<figure>
  <img src="/assets/projects/DinosaurMaze4.png" alt="Dinosaur Maze final screen" width="600">
</figure>

### How do we go from here?

The core tasks have been outsourced to AI. It can code and build, and quite remarkably so. The human is then the orchestrator and the judge.

We imagine. The AI Build. We scrutinize and put our verdict forth. 
