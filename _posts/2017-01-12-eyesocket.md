---
layout: post
title: Eye socket lengths across the taxa
tags: [stat, eye socket size, taxa]
---

Skull measurements from published drawing and images produced by experts in the field were collected. Eye socket length is defined as the maximum length of the socket, except for taxa in the digited tetrapod group featuring antorbital vacuities, for which the major axis of an ellipse fit to the orbit alone was used. We define skull length as the distance from the tip of the snout to the caudal margin of the postparietal bones, at their medial suture.


Skull images used can be found in the Supplementary Appendix.


Directory titled [fig03_socket_length](https://github.com/maciverlab/bigeye/tree/master/figs/fig03_socket_length) has the main code to plot eye socket sizes across taxa. The function named [fig03a_socketlength](https://github.com/maciverlab/bigeye/tree/master/figs/fig03a_socket_length writes a text file with calculated stat values (mean, standard deviation and sample size) ,creates two data files:

1. List of eye socket lengths for 4 groups (finned, finned-transitional, digited, and digited-aquatic)
2. List of orbit lengths for finned and digited tetrapods

and outputs and saves a pdf with the plot for absolute eye sizes in mm across the groups created by trait evolution.

In order to execute the code in Matlab, simply type:


``` Matlab
run fig03_socketlength
```

The output figure will be:

![Eye socket lengths across taxa]({{ site.url }}/assets/fig03.png)

Relative eye socket size was calculated as residuals from a phylogenetically informed regression of log10-transformed variables, averaged over the full set of 1,000 trees. Positive residuals indicate eye sockets larger than expected based on skull length, whereas negative residuals indicate eye sockets smaller than expected.As expected for a diverse group, not all tetrapods are at their respective peak, reflecting a normal evolutionary pattern where trait values are dispersed around the optimal value. The Bayesian OU findings show that there must have been a selective benefit from larger eye sockets in finned-transitional and digited tetrapods, but uncovering its basis requires modeling visual performance across likely environments.

The for each specie is saved in a csv file titled BMres.csv and is the output of the R script that can be found in folder [fig03b_data](https://github.com/maciverlab/bigeye/tree/master/figs/fig03b_data). The R script can be executed through the command line by typing:

```
$ Rscript gettingBMres.R —cwd
```

The species and corresponding residuals were then grouped according to the trait evolution. 


