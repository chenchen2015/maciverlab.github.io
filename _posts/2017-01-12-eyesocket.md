---
layout: post
title: Eye socket lengths across the taxa
tags: [stat, eye-socket-length, taxa]
---

Skull measurements from published drawing and images produced by experts in the field were collected. Eye socket length is defined as the maximum length of the socket, except for taxa in the digited tetrapod group featuring antorbital vacuities, for which the major axis of an ellipse fit to the orbit alone was used. We define skull length as the distance from the tip of the snout to the caudal margin of the postparietal bones, at their medial suture.


Skull images used can be found in the Supplementary Appendix.


Directory titled [fig03_socket_length](https://github.com/maciverlab/bigeye/tree/master/figs/fig03_socket_length) has the main code to plot eye socket sizes across taxa. The function named [fig03_socketlength](https://github.com/maciverlab/bigeye/blob/master/figs/fig03_socket_length/fig03_socketlength.m) writes a text file with calculated stat values (mean, standard deviation and sample size) ,creates two data files:

1. List of eye socket lengths for 4 groups (finned, finned-transitional, digited, and digited-aquatic)
2. List of orbit lengths for finned and digited tetrapods

and outputs a pdf with two plots:


1. Absolute eye size in mm across the groups created by trait evolution
2. Relative eye size with respect to skull length across the same set of groups

In order to execute the code in Matlab, simply type:


``` Matlab
run fig03_socketlength
```

The output figure will be:

![Eye socket lengths across taxa]({{ site.url }}/assets/fig03.png)

