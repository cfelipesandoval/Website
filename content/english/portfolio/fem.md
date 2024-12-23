---
title: "Numerical Electromagnetics"
date: 2024-05-01T12:14:34+06:00
image: "images/portfolio/fem/front.png"
# client: "John Doe"
project_url: "https://github.com/cfelipesandoval/cqemfem"
categories: ["Programming", "Physics"]
description: "This is meta description."
draft: false
---

<h4 class="text-center" style="font-size: 30px">
The Project
</h4>

For my capstone at Purdue, I worked on creating a Finite Element Method for Electromagnetics tool for the Computational Quantum Electromagnetics lab. The goal was to make an easily accesible tool that could calculate all the possible modes that may propagate in specific geometries.

<h4 class="text-center" style="font-size: 30px">
<br>How I made it
</h4>

To build up to the final 3D Potential Based tool, I began working my way up to understand the FEM for electromagnetics starting with the 1D case. 

A lot of the project's math was based off of Jin's textbook [Theory and Computation of Electromagnetic Fields](https://www.amazon.com/Theory-Computation-Electromagnetic-Fields-Jian-Ming/dp/0470533595).

<h4 style="font-size: 25px">
<br>1D Simulation
</h4>

<img src="/images/portfolio/fem/1d.png" class="postimage">

This is a plot made with the [1D-FEM](https://github.com/cfelipesandoval/cqemfem/tree/main/1D_FEM) numerical solver of a wave propagating into a different media at the center of the image. Although the colors could use some imporvement, the accuracy was surprisingly good for something I put together in a few hours.

The goal for this was just to learn more or less how the process would work for higher dimensions, however, I did not include any sort of object oriented concepts for this one as it seemed like overkill.

<h4 style="font-size: 25px">
<br>2D Simulation
</h4>

Here's a couple of pictures of what my [2D-FEM](https://github.com/cfelipesandoval/cqemfem/tree/main/2D_FEM) code does

<img src="/images/portfolio/fem/2d.jpg" class="postimage">

These are essentially plots of two modes that propagate through a slice of a rectangular waveguide with perfectly conducting walls.

To calculate the modes with the finite element method, a mesh of each waveguide with triangular elements is created in [Cubit](https://coreform.com/coreform-cubit/), and then fed into the program. In the repo, the "ReadAbaqusMesh.py" file deals with this part of the process.

<img src="/images/portfolio/fem/disc.png" class="postimage">

I thought this next one was cool, and proved to me that the code should (at least in theory) work for any arbitrary shape.

<img src="/images/portfolio/fem/2d_circ.png" class="postimage" style="max-width:400px">

<h4 style="font-size: 25px">
<br>3D Simulation
</h4>

Finally, the goal of this project was to reach the stage where the modes for a 3-dimensional cavity could be calculated with [3D-FEM](https://github.com/cfelipesandoval/cqemfem/tree/main/3D_Potential_FEM). This simulation was done in two ways, first with scalar basis functions for scalar, then with vector ones for a potential-based formulation.

The meshing process was similar as in the 2D case, where tetrahedral elements are used to discretize the cavities. 

For the potential-based formulation, my code calculates the contribution of each element with the help of an eigensolver. Each contribution has the form of a vector field, and in the end a plot can be made with the magnitudes of each vector.


<img src="/images/portfolio/fem/3d.png" class="postimage" style="max-width:400px">

This plot is made from two slices of the cavity on perpendicular axes.

<h4 class="text-center" style="font-size: 30px">
<br>Outcomes
</h4>

With the help of a few of the other people working on parallel projects, we presented at Purdue's Research Expo. This is an opportunity where undergraduate students participating in research can share their projects through a poster presentation.

Here's a picture of me at the poster presentation.

<img src="/images/portfolio/fem/presenting.jpg" class="postimage">

And here's the poster I made for it.

<img src="/images/portfolio/fem/presentation.png" class="postimage">