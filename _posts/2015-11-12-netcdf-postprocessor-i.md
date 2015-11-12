---
layout: post
title: "NetCDF postprocessor I"
description: ""
category: python
tags: [python]
---
{% include JB/setup %}

# Gridded NetCDF plotting tool 1

I'm working with a full scale general circulation model with atmospheric chemistry, and I get output from it in the NetCDF format, which is in wide use in large parts of the geosciences community. The format is excellent as far as I'm concerned, but there is always the problem of turning those raw output files into figures and numbers that can be presented. It seems everyone are making their own custom codes to process the output, and so I started out for myself learning to interact with the file format.

Most of my programming experience is in Matlab and C++, but when I started this project I decided to switch to python, mainly due to the open source nature of that language, and it's large community. So I started out thinking I would make a relativley general purpose plotting code for use with gridded NetCDF data. This is very much a work in progress, where I started out with a very naive structure, and this ended up being seriously clunky to use. I made all the figures in the poster in my previous post using the code, but I'm not very happy with it. 

I would like to rewrite it completely using the xray library for python, which allows indexing directly on named axes, thus simplifying the bookkeeping of axes, which was a major headache as I tried to expand the functionality of my first code. The problem is finding time to do it in between actually using the code to do research, and all of the other stuff we all have to do. Again this ties into the fact that most researchers make custom ad hoc code, that they don't maintain to a satisfactory degree. I actually want to make somthing that is eventually good enough that it could be a help for other students and researchers in  y group, not just some ad hoc scripts. 

Anyway, the code is available from my Github profile.