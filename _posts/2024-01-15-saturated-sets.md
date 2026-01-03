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

Thus if $C$ is open, so is its projection. This holds similarly for closed sets.

## Intuition

Intuitively, this is a way to get some of the nice properties of bijection without needing bijections.

## Example

**Example:** Find a quotient map which is not open.

It is easiest to think about discrete cases to avoid enumerating over classes. Additionally, we can think about the above fact and conclude that any domain which contains sets that are not saturated will fail to be open and closed on those sets. This means we need only a non-injective quotient map. Let $f$ be the map $x^2$ with the usual topology on domain and range.
