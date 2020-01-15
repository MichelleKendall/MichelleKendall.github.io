---
title: Trees with related tips
date: 2020-12-12
description: A way to compare trees with 'related' tips
categories:
  - metrics
  - phylogenetics
image: related_trees_teaser.png
author_staff_member: michelle
---

Our <a href="https://academic.oup.com/mbe/article/33/10/2735/2925548" target="_blank"> first tree metric</a>
was designed to compare two or more trees with identical tip labels - alternative evolutionary stories for the same set of organisms.
Sometimes it is helpful to compare trees whose labels are not related at all, for example a tree of flu virus samples from patients in New York versus a tree of flu virus samples from London. Differences in the shapes of the trees might tell you something about how the virus is adapting to differing evolutionary pressures in the two cities.

Here we address a sort of middle ground, where the tree labels are not identical across the trees but there is some relationship between them.
An example of this would be from genetic deep sequencing, where there are multiple "reads" per organism at each window (section) of the genome.
The tree built on the first window will have many tips for organism A, many tips for organism B, and so on, and the same is true for the tree built on the second window, as demonstrated here:

<img src="/images/related_trees_3_example.png" alt="">

The distinctions between organisms are fixed but the numbering of the reads is arbitrary, so that "read 1" for organism A in window 1 does not necessarily correspond to "read 1" for organism A in window 2 - we just know that they are both from organism A.
Nevertheless, it can be helpful to compare the trees across the windows.
We will outline our methods here; for the full details see our <a href="https://www.biorxiv.org/content/10.1101/251710v1" target="_blank"> bioRxiv preprint</a>.
