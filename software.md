---
layout: article
title: Software
permalink: /software/
image:
  feature: knitted_tree_banner.jpg
---

{% include toc.html %}

I maintain the R packages [*treespace*](#treespace) and [*phyloTop*](#phyloTop).

### *treespace* <a name="treespace"></a>

*treespace* is a package for statistical exploration of landscapes of phylogenetic trees. (Note, it was previously released with the name "treescape".) 
It includes a shiny app which provides a simple user interface for the functions. 
You can read more about the package in <a href="https://dl.dropboxusercontent.com/u/2767176/treespace.pdf" target="_blank">this vignette</a>. 
To install and load it, simply run (in R > 3.2.2):
```
install.packages("treespace")
library(treespace)
```
You can also:
* <a href="http://goo.gl/CuASjw" target="_blank">try out the treespace user interface</a> direct from your browser (no need to install R)
* find the stable R package <a href="https://cran.r-project.org/web/packages/treespace/index.html" target="_blank">on CRAN</a>, along with previous releases
* find the development version with all the latest updates <a href="https://github.com/thibautjombart/treespace" target="_blank">on GitHub</a>


### *phyloTop* <a name="phyloTop"></a>

In December 2015 I began maintenance of the package *phyloTop* for exploring topological properties of trees. It includes functions to calculate tree summary statistics (imbalance, depth, configurations sizes etc.), visualisation tools for highlighting topological properties of a tree in a plot (cherries, subtrees, ladders etc.) and tools for simulating an epidemic and its corresponding transmission genealogy. 
* it can be found <a href="https://cran.r-project.org/web/packages/phyloTop/index.html" target="_blank">here on CRAN</a> and can be installed and loaded by typing
```
install.packages("phyloTop")
library(phyloTop)
```
* the development version can be found <a href="https://github.com/MichelleKendall/phyloTop" target="_blank">here on GitHub</a> and installed and loaded using
```
devtools::install_github("michellekendall/phyloTop")
library(phyloTop)
```

Below is an example from the package. The command
```
subtreeShow(rtree(20), nodeList=c(23,35), mainCol="navy", 
        subtreeCol="cyan", nodeLabelCol="cyan", edge.width=2)
```
plots a random tree with 20 tips, and highlights in cyan the subclade(s) descending from internal nodes 23 and 35.

![phyloTop_example]({{ "/images/subtreeShowExample.png" | absolute_url }}) 