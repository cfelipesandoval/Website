---
title: "N-Body Orbit Simulator"
date: 2024-12-17T12:14:34+06:00
image: "images/portfolio/nbody/Figure8.gif"
# client: "John Doe"
project_url: "https://github.com/cfelipesandoval/N-Body_Simulator"
categories: ["Programming", "Physics"]
description: "This is meta description."
draft: false
---
<h4 class="text-center" style="font-size: 30px">
The Project
</h4>

During the end of my first semester as a grad student, I had to come up with a project to demonstrate my ability to create programs with numerical models for my Earth Systems Modelling course. I thought of the classic Three-Body Problem, but wanted to challenge myself, and decided to do it for an arbitrary number of masses.

I made a few simulations with 3blue1brown's renderer [Manim](https://github.com/3b1b/manim). 

This is a simulation of the solar system. The simulation was done with data from NASA's [planetary fact sheet](https://nssdc.gsfc.nasa.gov/planetary/factsheet/).

![image](images/portfolio/nbody/SolarSystem.gif)

For fun, I took the figure 8 orbit seen in the title, and made a simulation with four of them orbiting a central one. 

![image](images/portfolio/nbody/OrbitingFig8.gif)

You can check out the details of how you can use this tool in my [GitHub Repo](https://github.com/cfelipesandoval/N-Body_Simulator). 



<h4 class="text-center" style="font-size: 30px">
<br>Updates I want to Make
</h4>

Although the simulation is very quick already using Python, I would like to update it for the brunt of the computation to be done with C++. I want to essentially use Python as a wrapper and to make viualization easy to work with.