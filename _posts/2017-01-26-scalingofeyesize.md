---
layout: post
title: Scaling of eye socket size in early tetrapodstags: [tetrapods, eye size]
---

It is well known that eyes become proportionately smaller with an increase of body size. As the early tetrapods in our study feature quite disparate body sizes we need to account for these scaling effects. Figure S5 illustrates our efforts in this regard. We ran this over our entire set of trees.

In all cases, early tetrapods featured negative allometry of eye sockets compared to skull length. Trying to remove the scaling effects by dividing eye socket size by skull length therefore doesn’t remove this size bias, but calculating residuals successfully removed scaling effects. To run our code, open the terminal in folder [figExt_05](https://github.com/maciverlab/bigeye/tree/master/figs/figExt05_scaling) and type…following scripts…```$ Rscript figExt_05.R --cwd
```

These will output and save the following figure:

![Scaling of eye size]({{ site.url }}/assets/figExt05.png)