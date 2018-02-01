---
layout: post
title: "A really simple GCM part 1"
description: ""
category: models
tags: [models,thoughts, model code]
excerpt_separator: <!--more-->
---
{% include JB/setup %}

# [A really simple GCM part 1: A physicist meets modern Earth System Models.](http://hansbrenna.github.io/models/2018/01/26/simple-gcm)
Last spring, when I returned to work after my paternity leave, I felt frustrated that the GCM/ESM (CESM1) I'm using for my research is so damned complicated. It's very hard to get any kind of feeling for how the massive model actually works. Of course I could spend forever reading the code and technical documentation, but the full complexity makes it difficult to grasp, and I would not have enough time to spend on actually doing my own research.

Don't get me wrong, I like my model. It's just that I'm a little bit uncomfortable with using models I don't fully understand. I guess this is an aspect of a subtle cultural difference between meteorology and some other physical sciences [1]. Since I have about 6 years of training as a physicist I bring that cultural baggage with me into my climate science/meteorology work, and It's making me uncomfortable with the "black-boxiness" of modern Earth System Models. In the physics fields I trained in you're generalyy expected to build your own simulation code, and if you inherit some code you're usually inheriting it from the person who built it and you're expected to fully understand everything before using it. Needless to say, that's not how it works in modern meteorology.

<!--more-->

To ease my discomfort I picked up a couple of books on numerical methods for atmospheric modeling. These books generally avoid discussing the implementation of models utilizing the full set of primitive equations used in GCMs, and stick to discussing similar numerical methods applied to simpler systems of equations. I understand that the implementation of a full dynamical core with the rudimentary parametrizations needed for closure is a major task, especially if you want to use up-to-date numerical methods, so it's not unreasoable that this is not covered in textbooks. I would learn a lot by following these books in detail, but what I wanted (and still want) is a GCM so simple I can fully understand how it works.

When I had just started my PhD position i randomly picked up a book called "A vast machine. Computer models, climate data, and the politics of global warming" by Paul N. Edwards [2]. I felt out of my depth and very unfamiliar with meteorological data, climate science and the models used in my new field, and this was a brilliant introduction. There is a part in the book where Edwards tracks the development of the first numerical weather prediction models into general circulation models able to simulate what he calls "The Infinite Forecast", a simulation of climate rather than a weather forecast. There, I found references to the first and second generation of GCMs, which are vastly more primitive than modern ones, both in the processes they attempt to model and in the numerical methods used. 

By stripping away almost 5 decades of scientific and numerical progress, I finally found model descriptions I was able to follow in detail. These models generally use finite differencing as their numerical methods instead of the spectral or finite volume methods of most modern models. Finite differencing is much easier to understand, at least for me, as I have a fair bit of experience with it. The target for my intensive reading was the early models from NCAR from the late 1960s and early 1970s [3,4].

My decision was made almost instantly, I would like to try to re-implement a version of the early NCAR GCM, starting with the dry dynamics. I started with great optimism last spring, but quickly foud I was in over my head. Before Christmas I took it up again as a diversion while waiting for comments on my paper and my model tests to run. I was more thorough this time working more with pen and paper. In a series of posts I will trace my work on this problem. It will probably take some time, since I have to do this on my spare time, which I don't have a lot of, but turning this into a blogging project will probably help with my motivation

Stay tuned!

## References
1. Sundberg, M. Cultures of simulations vs. cultures of calculations? The development of simulation practices in meteorology and astrophysics. Stud. Hist. Philos. Mod. Phys. 41, 273–281 (2010).
2. Edwards, P. N. A Vast Machine: Computer Models, Climate Data, and the Politics of Global Warming. (MIT Press, 2010). doi:10.1111/j.1541-1338.2011.00522_3.x
3. KASAHARA, A. & WASHINGTON, W. M. NCAR GLOBAL GENERAL CIRCULATION MODEL OF THE ATMOSPHERE. Mon. Weather Rev. 95, 389–402 (1967).
4. Oliger, J. E., Wellck, R. E., Kasahara, A. & Washington, W. M. NCAR GLOBAL CIRCULATION MODEL. NCAR report (1970)