---
layout: post
title: "An Example Theorem with LaTeX"
date: 2024-01-20
categories: [Algebra, Number Theory]
---

This is an example post demonstrating how to use LaTeX in your math journal entries.

## Theorem: Sum of First n Natural Numbers

**Theorem:** For any positive integer $n$, the sum of the first $n$ natural numbers is:

$$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$$

### Proof by Induction

**Base Case:** For $n = 1$, we have:

$$\sum_{i=1}^{1} i = 1 = \frac{1 \cdot 2}{2}$$

So the formula holds for $n = 1$.

**Inductive Step:** Assume the formula holds for $n = k$, i.e.:

$$\sum_{i=1}^{k} i = \frac{k(k+1)}{2}$$

We need to show it holds for $n = k + 1$:

$$\sum_{i=1}^{k+1} i = \sum_{i=1}^{k} i + (k+1) = \frac{k(k+1)}{2} + (k+1)$$

Factoring out $(k+1)$:

$$= (k+1)\left(\frac{k}{2} + 1\right) = (k+1)\left(\frac{k + 2}{2}\right) = \frac{(k+1)(k+2)}{2}$$

This completes the inductive step. By mathematical induction, the formula holds for all positive integers $n$. $\square$

## Applications

This formula appears in many contexts:

1. **Combinatorics**: The number of ways to choose 2 items from $n+1$ items is $\binom{n+1}{2} = \frac{n(n+1)}{2}$

2. **Probability**: Expected value calculations often use this sum

3. **Analysis**: The formula is useful in approximating integrals

