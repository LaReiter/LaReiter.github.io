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

If you are curious about the game, please find the source code, game files and description <a href="https://github.com/LaReiter/Pygame-DinosaurLabyrint" target="_blank">on my Github</a>.

Here I will not go into details with the game, but rather explain my process of software development through collaboration with an AI.

### The game manifest

It all started with some imaginative thinking. I love mazes. My kid, and to some extent myself, love dinosaurs. Can we build a game of mazes and dinosaurs? Definetely. 

I wrote down my thoughts on how I imagined this game, from the visuals to the game mechanics. I wrote down my thoughts in a concise and structured way, that I knew any large language model (LLM) would be able to quickly decipher.

My thoughts - the game manifest - was saved as a .txt file inside a folder titled **Dinosaur Maze**. Based on this manifest, I already knew what this folder would eventually contain, and I began creating the subfolders.

**Note** My game manifest can also be found <a href="https://github.com/LaReiter/Pygame-DinosaurLabyrint" target="_blank">on my Github</a>.

### The graphics 

Besides a tree and tiles, I decided I wanted 3 cartoon figures in my game: an adventurous hero, a t-rex and a brachiosaurus. I wanted simple animations: two frames per movement cycle would do. 

Thus I would be needing 6 snapshots of these figures. Two frames for vertical movement (using reflection, we can cover both left/right movement). Two frames for upwards movement (with the back of the figure facing the viewer). Two frames for downwards movement (with the front of the figure facing the viewer).

To generate these figures, I used other large language models (LLMs) with integrated graphics-rendering capability.

But first I would be needing the right prompt. To that end, I had a short conversation with Claude, talking about how I imagined these figures. Among other details, I stressed that each frame should be distinct to fully capture a movement cycle. 

Eventually, Claude produced sufficiently detailed prompts for each figure, that I could then prompt to the graphics-rendering LLMs.

After repeating the prompts a few times and replying with some smaller adjustment requests, I was satisfied with the result.

Using the integrated background removal tool to of Photos (windows pre-installed), I was able to obtain transparent figure backgrounds necessary for in-game deployment. 

<figure>
  <img src="/assets/projects/DinosaurMaze2.png" alt="Dinosaur Maze level" width="600">
  <img src="/assets/projects/DinosaurMaze3.png" alt="Dinosaur Maze mechanics" width="600">
</figure>

### The implementation

Through Visual Studio (VS) Code, I navigated to my folder, which now contained the game manifest (readme.txt) along with all the graphics.

I used Claude Code as a plugin in VS to read the manifest, and search the folder to get an overview. I then asked Claude to make a plan for how to implement this game.

Claude Code came up with a plan, which we adjusted through a conversational back-and-forth.

Once I was satisfied with the plan, I requested that Claude Code wrote a readme.md file, that summarized our plan and also described everything relevant to the game (e.g. folder content, game mechanics).

Finally, I asked Claude to execute the plan and Claude responded by producing a set of auxilliary python files, and a main file to run the game.

The intial result was not perfect. The game didn't look impressive, and there were a couple of issues with the game mechanics.

Through a iterative and conversational process, these things were quickly fixed.

The idea of the game was conceived one early evening. The next evening, the game was done.

<figure>
  <img src="/assets/projects/DinosaurMaze4.png" alt="Dinosaur Maze final screen" width="600">
</figure>

### A lesson learned

Our role as a developer of software has changed fundamentally. 

The core tasks have been outsourced to AI, and coding skills are no longer necessary to succeed: The AI can code and build, and quite remarkably so. 

Instead the developer must see himself as an orchestrator and a judge.

We must imagine, and be creative. The AI will do the heavy-lifting and build our vision. But it will not nail it. We need to scrutinize what it is doing, judge its work and talk to it to make our vision clear as the day.

This if the future of the developer. And possible of many others.
