---
layout: post
title: "The story of SDYCORE LAB part 1"
description: ""
category: SDYCORE
tags: [models,thoughts, model code, SDYCORE]
excerpt_separator: <!--more-->
---
{% include JB/setup %}

# [The story of SDYCORE LAB part 1](http://hansbrenna.github.io/sdycore/2018/10/11/SDYCORE-story-1)

Like I've written about before, I have had a very strong interest in writing my own simple GCM/dynamical core. After several frustrating initial attempts, partly described [here](http://hansbrenna.github.io/models/2018/02/01/simple-gcm-1) I switched strategy. Rather than attempting to reimplement someone else's model from their description, I would start from the primitive equations and derive my own model, aiming for as much simplicity as possible in the system of equations.

By working in an isobaric (pressure) vertical coordinate, the equations become very simple, but implementing a non-flat surface becomes computationally hard, so I chose simplicity over realism here for the first try. The governing equations vere very neatly described in a 1974 paper by Akira Kasahara in Monthly Weather Review, called "[Various Vertical Coordinate Systems Used for Numerical Weather Prediction](https://journals.ametsoc.org/doi/10.1175/1520-0493%281974%29102%3C0509%3AVVCSUF%3E2.0.CO%3B2)".

The set of equations consist of 4 prognostic equations for horizontal wind, temperature and surface pressure which are extrapolated forward in time, and 3 diagnostic equations for vertical pressure velocity, pressure velocity at the surface and geopotantial height. In addition we need upper and lower boundary conditions. I'll get into the full derivation of the system of equations in a later post where I'll also go into details of the numerical scheme.

While I was at the EGU this year, I started working on deriving the discrete equations with pen and paper, and implementing them in Python. The targeted case was the standard dry dynamical core benchmark described in the 1994 article by [Held and Suarez](https://journals.ametsoc.org/doi/abs/10.1175/1520-0477%281994%29075%3C1825%3AAPFTIO%3E2.0.CO%3B2). Now the entire thing was quite transparent to me, finally and I was able to implement the basic equations in a few days. Now began the quest for numerical stability (this will be the title of a post coming soon).

This stage took me about a month, and the book "[Numerical Techniques for Global Atmospheric Models](https://link.springer.com/book/10.1007%2F978-3-642-11640-7)" was an invaluable resource, especially Chapters 3, 4 and 13. I tried different ways of obtaining linear and non-linear stability and suppressing computational modes, eventually getting stability over longer simulations.

This is where the project stands at the moment. On the way the numerical scheme has gotten a little more complicated than it started out as. But the 4th order dynamical core in the [SDYCORE LAB](https://github.com/hansbrenna/sdycore_lab) repository on GitHub is basically functional and reproduces the basic structure of the Held-Suarez flow pattern. There is something weird going on in the vertical velocity towards the poles, possibly related to an error in the pole condition, which I will have to look into, and the code is not as readable as I would like. I'm going to do a major restructuring of the code to enhance both performance and reliabilit, and I'll try to get the time for that relatively soon.
