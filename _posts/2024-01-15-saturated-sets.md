---
layout: post
title: "Saturated Sets"
date: 2026-01-03
published: true
categories: [Topology, Algebra]
---

## Introduction

Saturated sets: My instinct is to imagine that the definition of a saturated set is one that can be represented by the preimage of some set with respect to a quotient map. A quotient map is a "strongly continuous" map in which sets in the target space are open iff their preimages in the domain are open. 

Supposing $\pi$ is a quotient map, then if $C$ is a saturated set of an open set, then it is open; if it is the preimage of a closed set, it is closed. Furthermore, you can project $C$ via $\pi$ and its topological openness or closedness is preserved. 

The definition of a saturated set is that it contains every set it intersects. In this, I am assuming a non-injective map $\pi$ because this would be trivial otherwise. In this case, it needs to contain all points of the preimage. I suppose these points should share a name. Additionally, if $\pi$ is not injective on $C$, then there are subsets of $C$ such that $\pi(C) = \pi(A)$ and $A$ is a subset of $C$, but that $\pi^{-1}(\pi(A))$ does not equal $A$. This is lining up to say that the reason for saturated sets is that they are invertible with respect to $\pi$.

## Definition

A set $C$ is **saturated** with respect to a quotient map $\pi$ if and only if it contains all sets it intersects of the form:

$$\pi^{-1}(\{p\})$$

## Properties

**Property 1:** A set $C$ satisfies:

$$\pi^{-1}(\pi(C)) = C$$

if and only if $C$ is saturated with respect to $\pi$.

**Proof:** Suppose $C$ is not a saturated set:

$$C \text{ not saturated } \implies \exists g \in \pi^{-1}(p) \text{ such that } p \in \pi(C) \text{ and } g \notin C$$

Then the composition is strictly larger than $C$.

**Property 2 (Quotient maps):** The composition of a quotient map with its preimage on a set $A$ contains $A$. For saturated sets, they are equal; for unsaturated $A$, $\hat{A}$ contains missing points.

**Property 3:** Quotient maps restricted to saturated sets are open maps.

Let $C$ be a saturated set, then:

$$C = \pi^{-1}(\pi(C)) = \pi^{-1}(\pi(C))$$


## Nonexample
We have seen that quotient maps restricted to saturated sets are also open when restricted to saturated sets. This is because any open saturated set is exactly the preimage of its projection, and thus its projection must be open by the quotient propoerty. 

A quotient map q is open if and only if for every open set $U\subset X$ the saturation $\hat{U} = \pi^{-1}\pi(U)$ is open. 

Proof: 
Suppose the saturation of each open set is open. Let A be any open set in X 
$\pi(A) = \pi(\hat{A})$. Since $\hat{A}$ is assumed to be open as a saturation of an open set, and hte image of an open saturated set is open, $\pi(A)$ is open for any open A. 

We have shown that if the saturation of any open set is open, then a quotient map is open, we now show that if the saturation of any open set is not open, then then $\pi$ fails to be an open map. 

Suppose $\hat{U}$ is the saturation of an open set $U$ which is not open. Then by the definition of a quotient map, $\pi(U)$ is open iff the saturation of U is open, thus $\pi(U)$ is not open, and the map is not open. 

This shows the utility of saturated sets within the context of quotient maps. Preimages of singletons, have the capacity to grow, and this is in general a property of sets and maps: 

Let $A\subset X, f: X\mapsto Y$ then $A \subset f^{-1}f(A)$ if f is injective, then we hae equality in this property. Because we can restriact maps into their images, to create surjectivity, this is a very convenient way to to create bijections. 