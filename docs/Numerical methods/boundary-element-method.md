---
title: Boundary Element Method
parent: Numerical methods
nav_order: 3
---

# Boundary Element Method

The idea of the boundary element method (BEM) is quite simple: instead of solving the problem in the whole volume of the domain, we solve it on the boundary of the domain. This reduces the dimensionality of the problem, which means that the number of degrees of freedom (dofs) is significantly reduced. To illustrate this, let's consider a 3D cube uniformly meshed. Let's denote as $$n$$ the number of dofs in one direction.

In the FEM framework, the number of dofs in the whole volume is $$n^3$$, whereas in the BEM framework, the number of dofs is reduced to $$6n^2$$.

![image](/numenichal/assets/images/meshes/cube_2Dmesh.png) ![image](/numenichal/assets/images/meshes/cube_3Dmesh.png)