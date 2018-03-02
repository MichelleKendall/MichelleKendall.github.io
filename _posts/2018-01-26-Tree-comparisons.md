---		
 layout: article
 title: Tree comparisons
 categories: blog
 excerpt: Why do we need to be able to compare trees in biologically meaningful ways?
 image:
  teaser: phylocladus_teaser.JPG
  feature: jacaranda_banner.JPG
---		

Much of my postdoctoral research in 2014-2018 was concerned with tree comparisons. Here's a brief overview of the problems which make tree comparison important, and what we've contributed to address the problems.

### The problem:

When studying a group of organisms, researchers can gain valuable information by knowing the evolutionary tree or *phylogeny* which relates them to each other. A phylogeny is a diagram which shows the ancestral links between a set of organisms. The <a href="http://www.onezoom.org/" target="_blank">onezoom</a> project is a great way to explore what we know so far about the entire tree of life. Typically, researchers are interested in a much smaller part of it, such as the tree of mammals, or the tree of a single virus, tracking the evolution of different strains.

Of course, apart from a few rare cases where evolution is happening within a short time frame and we can observe all the mutations, we usually do not know the tree for certain but have to *infer* the historical tree from what we see today. This can be achieved by *inference methods* which use DNA sequences (and lots of other things which are known about the organisms) to try to produce credible trees. This is more difficult than it might sound! Some of the problems are:
* there can be confusing signals in the DNA, making it hard to choose a tree which fits. Some of these are caused by errors or not having enough data, but some are caused by confusing evolutionary processes like [convergent evolution](https://en.wikipedia.org/wiki/Convergent_evolution), where different lineages (organisms from different parts of the tree) develop the same mutations.
* the assumptions you make (for example, if you think mutations happen at a fairly constant rate) can dramatically alter the results
* there are LOTS of possible trees. To give you an idea: if you have 10 organisms then there are about 34.5 million possible tree shapes to choose from. For 52 organisms there are about 275,000,000,000,...,000 (I've omitted 69 zeroes) possible tree shapes, which is more than the estimated number of atoms in the universe. And that's before you worry about setting the lengths of the branches in the tree to represent evolutionary timescales, which then makes the number of possible trees infinite. Researchers commonly study trees for hundreds or even thousands of organisms.

Perhaps not surprisingly, then, different inference methods can produce markedly different trees. Sometimes even a very small change in the input choices can lead to very different trees in the output. Some methods produce a single tree, others suggest thousands of possible trees, each of which is essentially equally likely to be correct.

### The (partial) solution:

My work with [Caroline Colijn](https://www.imperial.ac.uk/people/c.colijn) has been to develop ways to compare trees to give an idea of how similar or otherwise they are. Doing this "by eye" is notoriously difficult, partly because of how many possible shapes there are, and because it's quite hard to "read" trees quickly. Thankfully, computers can read them much quicker than humans. When trees are very dissimilar it can be hard to make any sense of them; our *treespace* software will classify them into groups of similar trees and find an "average" tree per group as a way of summarising the possibilities.

Where inference methods have not agreed on a single tree, our method has helped to identify the distinct, credible alternative evolutionary histories supported by the data. In <a href="http://www.anoleannals.org/2016/07/05/resolving-phylogenetic-uncertainty-in-anoles-using-treescape/" target="_blank">this blog post</a> there's an example of this application of our method to understanding the evolution of anole lizards. The method can also help to identify the sources of the uncertainty. For example, sometimes it is hard to represent the evolutionary relationships of organisms with a tree because *the evolution wasn't really tree-like*. Processes like recombination can mean that branches of the tree sometimes join up again, and then the inference method will struggle to make a tree fit the data. Our method helps to uncover these strange, conflicting signals in the data.

You can read more about all of this in our <a href="/publications" target="_blank">recent papers</a> and play with the *treespace* software <a href="shiny.imperial-stats-experimental.co.uk/users/mlkendal/treespace" target="_blank">here</a>.

### Extensions

We have also made various extensions of this work to address particular tricky cases. I hope to blog about them in the future. They include:
* emphasising the positions of a few "important" tips of interest
* drawing a pair of trees so that their key differences are highlighted
* a method to compare trees which represent the transmission of disease - a record of who infected whom
* methods to compare trees in instances where the labels at the tips do not match
