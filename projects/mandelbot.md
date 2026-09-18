---
layout: project
type: project
image: img/mandelbot/multibrotfifthpower.png
title: "Mandelbot"
date: 2021
published: true
labels:
  - Node.js
  - Discord.js
  - JIMP
  - Mathematics
summary: "A Discord bot for generating Mandelbrot and Julia set fractals through text commands."
---

<div class="text-center">
  <img width="600px" src="../img/mandelbot/mandelbot-discord-output.png" >
</div>

<div class="text-center p-4">
  <img width="200px" src="../img/mandelbot/julia0.png" class="img-thumbnail" >
  <img width="200px" src="../img/mandelbot/julia1.png" class="img-thumbnail" >
  <img width="200px" src="../img/mandelbot/julia2.png" class="img-thumbnail" >
</div>

[Mandelbot](https://github.com/maximovicente/Mandelbot) was a passion project of mine developed throughout late 2021 that began after the topics of mathematical fractals and universality piqued my interest. The aim of the project was to familiarize myself with implementing algorithms to tranform abstract mathematical expressions into images, and to gain experience with the JS image processing library [JIMP](https://github.com/jimp-dev/jimp). After figuring out the specific math- and JIMP-related functions necessary to generate static images, I found that the gradients in these images, whose steps were based on the number of iterations required for a specified Mandelbrot/Julia equation to diverge past certain bounds, could be represented in motion by rendering each iteration of the equation as a separate frame. The resulting animations, when generated for the standard Mandelbrot set or a specific Julia set, I find to be quite beautiful. An example can be seen below. 

<div class="text-center">
  <img src="../img/mandelbot/boomerang_1.gif" >
</div>

I also recommend checking out Movie Vertigo's [Mandelbrot Iteration](https://www.youtube.com/watch?v=pD7_n5gCUPI) video on YouTube, showing more smoothly the kinds of visuals these fundamental mathematical expressions can produce. If you are interested in learning more about these fractals and the math that governs them, there are plenty of resources on the matter, but I suggest starting with [2swap's video on the matter](https://www.youtube.com/watch?v=Ed1gsyxxwM0).