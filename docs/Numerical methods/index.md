---
title: Numerical methods
---
# Numerical methods

In a perfect world, we would be able to solve all the problems we encounter using analytical methods. For exemple, let's take a beem loaded by a force with two main hypotheses: 

1. During the deformation, the cross-section stay perpendicular to the neutral axis of the beam.
2. There is no relative rotation between the cross-section of the beam.

These two hypotheses are called the Euler-Bernoulli hypotheses and are the basis of the Euler-Bernoulli beam theory.

![image](/numenichal/assets/images/euler-bernoulli-hyp.png)

In mechanical engineering, numerical methods are essential for solving complex problems that cannot be addressed analytically. These methods involve the use of algorithms and computational techniques to obtain approximate solutions to mathematical models. Numerical methods are widely used in various fields of mechanical engineering, including structural analysis, fluid dynamics, heat transfer, and optimization.

```mermaid
graph LR;
    accTitle: the diamond pattern
    accDescr: the diamond pattern
    id1[Physical Problem] --> id2[Numerical Solution] & id3[Numerical Solution];
    id2[Numerical Solution] --> id3[Numerical Solution];
    id3[Mathematical Abstraction] --> id2[Numerical Solution];
```

This diagram illustrates the iterative process of numerical methods in a historical context. First, a physical problem is defined. From this problem that we want to solve, engineers and physicists try to solve it using computers. Often, numerical solutions work first without any mathematical abstraction. It is the pragmatic soul of engineers. Then, mathematicians try to find a mathematical model that can be solved using numerical methods, to give a more general, systematic and rigourous frame for both the physical model and the numerical method to solve it.

There exist several numerical methods, each with its own advantages and limitations. Some of the most commonly used numerical methods in mechanical engineering include:

## Finite Element Method (FEM)

The idea of the finite element method is to divide a complex structure (with its geometry) into smaller, simpler parts called finite elements.

## Boundary Element Method (BEM)
## Finite Difference Method (FDM)

# HTML blocs

## Pluto.jl notebook example

<iframe src="/numenichal/assets/notebooks/pluto_example.html"
        width="100%"
        height="600px"
        frameborder="0">
</iframe>