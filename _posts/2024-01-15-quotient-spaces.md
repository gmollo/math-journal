---
layout: post
title: "Quotient Spaces"
date: 2026-01-03
published: true
categories: [Topology, Algebra]
---

Continuing from the discussion of saturated sets, I am hoping to flesh out all properties of quotient spaces based on the construction of them before getting to its definition, so that most properties seem almost obvious.

## Definition: Closed Map

Given a pair of topological spaces $X, Y$, a map $c$ is **closed** if for each closed $L$ in $X$, $c(L)$ is closed in $Y$.

$$L \in \tau_X^c \implies c(L) \in \tau_Y^c$$

## Constructing Quotient Maps

These and open maps give clever ways to construct quotient maps. For instance, if $f$ is continuous and open, then you know that preimages of open sets are open sets, and that images of open sets under $f$ are open sets, thus $f$ is a quotient map. 

If you instead supposed that $f$ was closed, you could use complements, and use the preservation of closedness under preimages of continuous maps to infer that $f$ was a quotient map from the alternative definition.

$$f \text{ continuous } \land (f \text{ open } \lor f \text{ closed}) \implies f \text{ quotient}$$

Lets get the terms clear for maps from $X \to Y$
Continuous: 
$$f^{-1}(U) is open/closed if U is open/closed resp. $$
Surjective:
$$f^{-1}(p) \neq \emptyset for p \in Y $$
Quotient:
$$f^{-1}(U) is open/closed **if and only if** U is open/closed resp. $$
Open:
$$f(U) is open if U is open $$
Open:
$$f(U) is closed if U is closed $$

We have many nice properties here, but we still do not enough to sort of say "open sets go to open sets". Even in a quotient map, any non-saturated set open set need not map to an open set unless its saturation is also open. 

# The Quotient Topology 
In the event that we have gotten tired of trying to think up interesting examples for quotient maps, we can resort to using the quotient topology, and the following quotient space construction. 

Def: Given a map from X $\mapsto$ Y, and $\pi$ is any surjective map, we can choose the precise topology on Y such that $\pi$ is a quotient map (by taking exactly those sets in Y whose preimages are open in X and calling them open). This induced collection is a topology because of the nice properties of unions and intersections commuting with preimages, and loafing off of the properties in X. 

The **quotient space** is what you get when you map a topological space onto a partition of itself and equip the partition space with the quotient topology. Of course, this $\pi$ does not feel continuous in any meaningful way as the cardinality of the spaces is often not the same, but that's math. It is useful to remember the picture of the saturation as we move forward. The saturation emphasized those sibling points that may or may not get left begind when you initially project forward via a quotient map, and it further leaves the impression that the pullback of points (or equivelance classes) can be a vast collection, or a finite one, but that there are many cases to consider. These pictures form a substantive portion of material later on. 

## Quotients restrict to quotients on saturated subspaces*
If the restriction set is open or closed this is true. It is true as well if $\pi$ is either an open or closed map, which quotients need not be. 

# Discussion. 
It has been some time since I studied point set topology. In particular, I do not much remember the properties used to distinguish non-homeomorphic spaces beyond the examples heavily citied in differential topology and analysis, in particular, the sorts of mesasurability arguments of the real line, which are analytic and not topological. One of the main points of homotopy theory, and for homology theory in general is to distinguish spaces based on derivable characteristics. To this end, it seems valuable to refresh myself on the elementary topological properties which inform much around euclidian spaces.
