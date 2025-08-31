---
title: "N-Body Orbit Simulator"
date: 2024-12-17T12:14:34+06:00
image: "images/portfolio/nbody/Figure8.gif"
# client: "John Doe"
project_url: "https://github.com/cfelipesandoval/N-Body_Simulator"
categories: ["Programming", "Physics"]
description: "This is meta description."
draft: true
---
<h4 class="text-center" style="font-size: 30px">
The Project
</h4>

During the end of my first semester as a grad student, I had to come up with a project to demonstrate my ability to create programs with numerical models for my Earth Systems Modelling course. I thought of the classic Three-Body Problem, but wanted to challenge myself, and decided to do it for an arbitrary number of masses.

I made a few simulations with 3blue1brown's renderer [Manim](https://github.com/3b1b/manim). 

This is a simulation of the solar system. The simulation was done with data from NASA's [planetary fact sheet](https://nssdc.gsfc.nasa.gov/planetary/factsheet/).

<img src = "/images/portfolio/nbody/SolarSystem.gif" class="postimage">

For fun, I took the figure 8 orbit seen in the title, and made a simulation with four of them orbiting a central one. 

<img src = "/images/portfolio/nbody/OrbitingFig8.gif" class="postimage">

You can check out the details of how to use this simulator in my [GitHub Repo](https://github.com/cfelipesandoval/N-Body_Simulator).


<h4 class="text-center" style="font-size: 30px">
<br>N-Body Problem Report
</h4>

Part of the Earth Systems Modelling class was to write a full report about the simulator. In it, I explain the theory to numerically solve 2 and 3 body problems, and extend it to an arbitrary number of bodies. Moreover, there is some insight into some of the simulator parameters and into the simulation error over time. 

<embed src="/images/portfolio/nbody/report.pdf" 
       type="application/pdf"
       frameBorder="0"
       scrolling="auto"
       height="768px"
       width="100%"/>

<h4 class="text-center" style="font-size: 30px">
<br>Updates I want to Make
</h4>

Although the simulation is very quick already using Python, I would like to update it for the brunt of the computation to be done with C++. I want to essentially use Python as a wrapper to make viualization easy to work with rather than doing the actual calculations as it is not as fast as I want it to be. 