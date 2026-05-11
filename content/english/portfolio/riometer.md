---
title: "Riometer"
date: 2025-05-11T00:00:00+00:00
image: "images/portfolio/riometer/auroraplane.jpg"
# client: "John Doe"
# project_url: "https://github.com/cfelipesandoval/cqemfem"
categories: ["Research", "Circuits"]
description: "This is meta description."
draft: true
---

Radio is one of the most important and widely used modern inventions. Pretty much all wireless technologies use radio in one way or another: from remote control, long-range communications, and navigation systems, our world depends on radio. Because of this, it is imperative that we are able to detect and monitor any deviations that could affect or compromise the effectiveness of such systems, and one major factor that determines this is the Earth's ionosphere.

<h4 style="font-size: 30px">
The Ionosphere
</h4>

If you haven't heard of the ionosphere, let me tell you about it (it's really cool). The ionosphere is the layer directly above the Earth's atmosphere that is hit by high energy X-rays from solar radiation. We owe it to this layer that we are not constantly bombarded by X-rays on Earth's surface. This effectively separates the electrons from the protons in atoms, creating a plasma. We call this process ionization, and it through this that we creatively get the name: The <b>Ionosphere</b>.

Depending on the altitude, we primarily separate the ionosphere into the D, E, and F regions, characterized by their differing neutrals and electron densities. 

<div class="postimage">
  <img src="/images/ionosphere/layers.png" style="width:100%">
  <h1 class="text-left" style="font-size: 10px">
  </h1>
</div>

For this article, I will focus primarily on the D-region, since most radio wave absorption occurs here.

<h4 style="font-size: 30px">
The D-region and its Importance
</h4>

Spanning between ~60 - 90 km ASL, as the lowest part of the ionosphere, the D-region is characterized by the high amount of neutral atoms still present. Because of these neutrals, there is a lot of radio wave absorption, especially for High Frequency and Very High Frequency waves (1 - 100 MHz). Due to relatively low electron densities here, there is great variability due to solar events, and even the day/night cycle.

Historically, it has been really difficult to measure since it is <i>too high for weather balloons and too low for satellites</i>. Really, the best measurements we've got of it are of [rockets sent shooting through it](https://www.gi.alaska.edu/news/third-2026-mission-launches-poker-flat-research-range). Because of this, multiple teams have developed clever tools to make measurements of this layer. Recently, there have been many efforts to utilize radio emissions [from lightning strikes to generate tomographies of the D-region](https://lf.gatech.edu/). In this article I will describe an instrument that I have been developing that uses noise from the universe to make measurements of this layer.

<h4 style="font-size: 30px">
What is a Riometer?
</h4>

This instrument's name, as mysterious as it may sound, is in fact just an accronym: The <b>R</b>elative <b>I</b>onospheric <b>O</b>pacity <b>Meter</b>. This instrument dates back to the 1950's, where radio scientists figured that they could use the radio noise produced by the big-bang and other sources in space to remotely sense the D-region of Earth's ionosphere. To measure the D-region, this tool "listens" to the amount of noise coming in from the universe, passing through the ionosphere, and catalogues how it changes over time. If we assume that the cosmic radio noise power is uniform, we can extract the electron density of the D-region by comparing measurements to determine the absorption that must have occurred. 

<h4 style="font-size: 30px">
What it Takes to Make a Riometer
</h4>

Like any radio remote sensing device, making a riometer requires a system that can sense very faint electromagnetic signals. To do so, the general approach is to use an antenna to pick up the signals, and a radio frequency (RF) front-end to clean-up, amplify, and collect the resulting data. Below is a very simple diagram of what a Riometer front-end (and most RF frontends) would look like.


<div class="postimage">
  <img src="/images/portfolio/riometer/simplediagram.png" style="width:100%">
  <h1 class="text-left" style="font-size: 10px">
  </h1>
</div>

Going through the system, there is:
1) (1) An antenna to pick up noise power
2) (2) An RF swtich to switch between the antenna and calibration signals
3) (3) A bandpass filter to remove any unwanted signals
4) (4) A low noise amplifier to increase the signal's power while adding very little noise to it
5) (5) A second amplifier to increase the signal to easily detectable levels
6) (6) A module to digitize data for postprocessing
7) (7) Somewhere to pick up and store the data 

<h4 style="font-size: 30px">
Site Testing
</h4>

Recently, I set up my prototype system at a farm in rural Tennessee and collected data for a period of around 24 hours. This experience was more illuminating that I would have liked, as I have learned the many downfalls of my system, but also the incredible successes that have come from it.

For this test, I set up some of the VLF antenna stands my lab uses, but repurposed them to create a 2-channel cross dipole configuration. I also used a pelican case to house all the front-end electronics.

<br>
Here's as picture of me and my antennas:

<div class="postimage">
  <img src="/images/portfolio/riometer/meandantennas.jpg" style="width:50%">
  <h1 class="text-left" style="font-size: 10px">
  </h1>
</div>

And here's a picture of me setting up the electronics to work:

<div class="postimage">
  <img src="/images/portfolio/riometer/settingup.jpg" style="width:80%">
  <h1 class="text-left" style="font-size: 10px">
  </h1>
</div>

<h4 style="font-size: 30px">
Future Work
</h4>

The single antenna system is essentially done and harware for my design will be frozen by the end of June of this year. However, the idea of this system is to create an array of this system to be able to take 2-dimensional planar images of the D-region. The multi-channel, multi-antenna array setup still needs to be finalized and I will be updating this post as that occurs, so watch out for it!