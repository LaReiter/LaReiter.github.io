---
title: "Paper planes"
image: "/assets/projects/paper-thumbnail.png"
mathjax: true
layout: post
excerpt: "Origami: Folding paper planes and a bit of statistics."
date: 2025-10-18
lang: en
---

<figure style="text-align: center;">

  <div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 10px;
    align-items: center;
  ">
    <img src="/assets/projects/paper1.jpg" style="width: 100%; height: auto;">
    <img src="/assets/projects/paper2.jpg" style="width: 100%; height: auto;">
    <img src="/assets/projects/paper3.jpg"  style="width: 100%; height: auto;">
    <img src="/assets/projects/paper4.jpg"  style="width: 100%; height: auto;">
    <img src="/assets/projects/paper5.jpg"  style="width: 100%; height: auto;">
    <img src="/assets/projects/paper6.jpg"  style="width: 100%; height: auto;">
    <img src="/assets/projects/paper7.jpg"  style="width: 100%; height: auto;">
    <img src="/assets/projects/paper8.jpg"  style="width: 100%; height: auto;">
  </div>

  <figcaption style="margin-top: 12px; font-style: italic; font-size: 0.95em;">
    Some of my (re)creations showing different types of paper planes. Some are small, some are big. Some are pointy, and some have large wingspans. Finally, some are bionic and flaps their wings like a bird or bat. The paper plane with the rockets has limited flight capability but looks amazing.
  </figcaption>

</figure>

As a kid I loved to fold paper airplanes. So much, that I bought myself a textbook on the mechanics and aerodynamics of paper planes. The book also included several colorful templates to be used. Now that my kid has reached the same age and independently shown an interest in the subject, I’ve found it deeply satisfying to revisit my old hobby.

Despite my satisfaction in simply folding the planes, the academic within me wanted to do some experimenting. So I decided I wanted to test how size and the number of wing folds influence flight.

I quickly realized, that coming up with a proper experimental design (reducing variance and bias) was non-trivial and time consuming. So instead, this project became about executing a simple (naive) design as a lesson in poorly conducted research. 

## The experimental design

I stand with my back to the dishwasher. In front of me is a sofa placed against a wall. At one end of the sofa, lying on the armrest, there is a pillow that serves as the target (right image below).

I alternate between throwing the four paper airplanes: (large, small) × (unfolded, folded). See left image below. If the airplane hits/do not hit the target (H), a score of 1/0 is recorded. If the airplane have/do not have a range far enough to reach the target (R), a score of 1/0 is recorded. If the airplane lands within/outside the width of the sofa at the time of landing, it is considered accurate (A), and a score of 1/0 is recorded.

The experiment is repeated 20 times for each plane.

I throw from shoulder height and attempt to use the same force and arm movement for every throw. Prior to each throw, I count down from three before swining my arm forward towards the target.


<figure style="text-align: center;">

  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; align-items: center;">
    <img src="/assets/projects/paperplanes.jpeg" style="width: 100%; height: auto;">
    <img src="/assets/projects/paperplane_target.png" style="width: 100%; height: auto;">
  </div>

  <figcaption style="margin-top: 12px; font-style: italic; font-size: 0.95em;">
    Left: The four paperplanes of the study (after the trial). Right: The experimental area, with definitions of binary variables precision P, range R and hit H.
  </figcaption>

</figure>


