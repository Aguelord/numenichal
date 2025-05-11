---
title: Numerical methods
---
# Numerical methods

In a perfect world, we would be able to solve all the problems we encounter using analytical methods. For example, let's take a beam (modelled as a one dimensional object) loaded by a force with two main hypotheses: 

1. During the deformation, the cross-section stays straight and perpendicular to the neutral axis of the beam.
2. There is no relative rotation between the cross-section of the beam.

These two hypotheses are called the **Euler-Bernoulli hypotheses** and are the basis of the Euler-Bernoulli beam theory. A last hypothesis is the so-called small deformation hypothesis, which states that the deflection of the beam is small compared to its length. This means that the angle of rotation of the beam is small and can be approximated by :

$$\theta(x) = \frac{\mathrm d\delta}{\mathrm dx}, \quad \theta^2\approx 0$$

Which is a first-order approximation of the angle between the tangent to the beam and the horizontal axis. 
In this equation, $$\theta(x)$$ is the angle of rotation of the beam at point $x$ and $\delta$ is the deflection of the beam, which is the **vertical displacement** of the beam at point $x$. Note that point $x$ is, for instance, the curvilinear abscissa of any point on the beam. This is useful to stay in a 1D framework and scalar functions.

![image](/numenichal/assets/images/euler-bernoulli-hyp.png)

Then, the Euler-Bernoulli relation, that relates the deflection of the beam to the applied load, is given by:

$$\frac{\mathrm d^2}{\mathrm dx^2}\left(EI\frac{\mathrm d^2\delta(x)}{\mathrm dx^2}\right)=q(x)$$

Where $q$ is the distributed load applied to the beam, $E$ is the Young's modulus of the material, and $I$ is the moment of inertia of the beam's cross-section.

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