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
    Figure: Some of my (re)creations showing different types of paper planes. Some are small, some are big. Some are pointy, and some have large wingspans. Finally, some are bionic and flaps their wings like a bird or bat. The paper plane with the rockets has limited flight capability but looks amazing.
  </figcaption>

</figure>

As a kid I loved to fold paper planes. So much, that I bought myself a textbook on the mechanics and aerodynamics of paper planes (the book also included several colorful templates). Now that my kid has reached the same age and independently shown an interest in the subject, I’ve found it deeply satisfying to revisit my old hobby.

Besides my satisfaction in simply folding the planes, the academic within me wanted to do some experimenting. So I decided I wanted to test how plane size and the number of wing folds influence flight.

I quickly realized, that coming up with a proper experimental design was non-trivial and ideally required several tools. So instead, this project became about executing a simple (naive) study design, and then playing the role of the critical reviewer of my own work.

## The (poor) experimental design

I stand with my back to the dishwasher. In front of me is a couch placed against a wall. At one end of the couch, lying on the armrest, there is a pillow that serves as the target of my plane (right image below).

I now alternate between throwing the four paper planes: (large, small) × (standard, extra fold). "Extra fold" means that I have folded the wings one more time compared to the standard plane. See the left image below. 

The planes are thrown 20 times each. I throw from shoulder height and attempt to use the same force and arm movement for every throw. Prior to each throw, I count down from three before swining my arm forward towards the target.

If the plane hits/do not hit the target (H), a score of 1/0 is recorded. If the plane have/do not have a range far enough to reach the target (R), a score of 1/0 is recorded. If the plane lands within/outside the width of the couch, it is considered accurate (A), and a score of 1/0 is recorded.

<figure style="text-align: center;">

  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; align-items: center;">
    <img src="/assets/projects/paperplanes.jpeg" style="width: 100%; height: auto;">
    <img src="/assets/projects/paperplane_target.png" style="width: 100%; height: auto;">
  </div>

  <figcaption style="margin-top: 12px; font-style: italic; font-size: 0.95em;">
    Left figure: The four paperplanes of the study (after the trial). Right figure: The experimental area, with definitions of binary variables precision P, range R and hit H. The dashed circle is the target pillow $H=1$. Planes that landed inside the couch were accurate $A=1$. Planes that reached the white pillow and beyond had good range $R=1$.
  </figcaption>

</figure>

## The findings

In the below Figure I have visualized the results of the experiments along with Wilson score 95\% confidence intervals on the proportions. It may appear that planes with an extra wing fold are more accurate (the paper stays near the couch), but have less range and are less likely to hit the target. 

<figure style="text-align: center;">

  <div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 10px;
    align-items: center;
  ">
    <img src="/assets/projects/paper_plot_A.png" style="width: 100%; height: auto;">
    <img src="/assets/projects/paper_plot_R.png" style="width: 100%; height: auto;">
    <img src="/assets/projects/paper_plot_H.png"  style="width: 100%; height: auto;">
  </div>

  <figcaption style="margin-top: 12px; font-style: italic; font-size: 0.95em;">
    Figure: Some of my (re)creations showing different types of paper planes. Some are small, some are big. Some are pointy, and some have large wingspans. Finally, some are bionic and flaps their wings like a bird or bat. The paper plane with the rockets has limited flight capability but looks amazing.
  </figcaption>

</figure>

Using Fisher's exact test, I tested the claims formally. I found that adding an extra wing fold had a significant impact on the outcome of range R ($p=0.003$) and hit chance H ($p = 0.016$) for large planes only. For other combinations of planes and outcomes, the impact of an extra fold was non-significant. P-values are Holm adjusted. 

## The devils reviewer: bias and variance

As stated earlier, I was not at all happy with this design. But I also love data collection and analysis, so here I are. Also, I realized that this could be a lesson on the importance of a good study design.

So what is wrong?

For starters, the sample size (20 throws per plane) only allow us to reliably detect large effects, and a formal test on the interaction between fold and size would be underpowered, and was therefore omitted.

Secondly, the measures are poor. I measured the range (R), whether I hit the target (H), and if the plane lands on the couch as a marker of accuracy (A). Obviously, A and R will be predictive of H, making $H$ slightly superfluous. Secondly, a plane can follow a chaotic route and still land on the couch, now being labelled accurate $A=1$. On the other hand, planes that curve slightly left will hit the wall, and are now inaccurate $A=0$ and fall short of the target $R = H = 0$. Binary variables also masks useful (quantitative) information: how far did it fly? how accurate was it? 

Regarding the planes, it seems unreasonable to expect that the planes only differ in the two dimensions "wing folds" and "size". There are neccesarily small deviations in how they are folded, that will have some impact on their ability to fly (well). Ideally, to avoid bias from our four planes with unique features/deviations, the throws should use a new folded paper plane of the type (i.e. size and wing fold). This also removes the risk, that I damage or deform the four planes through repeated throws.

Last, and by no means least, the throws were not perfectly identical. While I did my best to keep force and arm movement fixed, there are bound to be some variation between throws. Also, the point of contact between my hand and the plane was not fixed, and could vary from throw to throw.

So at the end of the day, this small experiment have some major caveats, which makes the results hard to interpret and, to be honest, slightly silly.

This small project, besides being fun to do, also serves as a lesson in the importance of dedicating enough time to creating a robust study design, such that later analysis and results remain interpretable, unbiased and useful.


