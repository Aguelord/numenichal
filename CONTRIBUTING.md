<!-- omit in toc -->
# Contributing to numenichal

First off, thanks for taking the time to contribute! ❤️

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. It will make it a lot easier for us maintainers and smooth out the experience for all involved. The community looks forward to your contributions. 🎉

> And if you like the project, but just don't have time to contribute, that's fine. There are other easy ways to support the project and show your appreciation, which we would also be very happy about:
> - Star the project
> - Tweet about it
> - Refer this project in your project's readme
> - Mention the project at local meetups and tell your friends/colleagues

<!-- omit in toc -->
## Table of Contents
- [I Have a Question](#i-have-a-question)
  - [I Want To Contribute](#i-want-to-contribute)
  - [Reporting bugs](#reporting-bugs)
  - [Suggesting enhancements](#suggesting-enhancements)
  - [Conventions for contributing](#conventions-for-contributing)
    - [Programming in Julia](#programming-in-julia)
    - [Latex](#latex)

## I Have a Question

If you have a question, make sure that you haven't found an existing topic in [Discussions](https://github.com/Aguelord/numenichal/discussions) and in the following paragraphs. If you can't find an answer there, please open a new discussion. We will be happy to help you. We are all learning together, and we are happy to help you. Your question may also help others in the future ; it can be about the course itself, the code, theorical aspects, a question about contributing, or anything else related to the project.

### I Want To Contribute
If you want to contribute, please read the [Code of Conduct](CODE_OF_CONDUCT.md) first. As you see, this project is open source and welcomes contributions from everyone, but you have to have some competence in one or more of the following topics :
- **Numerical methods and programming**, especially in the following fields.
- Applied mathematics, especially in the field of numerical methods and **functional analysis**
- **Mechanical, aeronautical, civil** or any other engineering field
- Other fields of physics may also be relevant, like **electromagnetism, thermodynamics**, etc. as they are also fields that are used by engineers.
- (If you have some historical knowledge or appetite about sciences and epistemology, it would be also great 👀)

As you see, the list is wide 🙂. The idea is that everybody can developp / add a subject about his topics, while maintaining a common framework with the rest of the project, especially the website. At the moment, the final product is **the website**.

### Reporting bugs

If you find a bug, please open an issue on GitHub, after checking that it hasn't already been reported in the [issues](https://github.com/Aguelord/numenichal/issues). It can be about some code that doesn't work, a problem with the website (a broken link, latex that doesn't render, etc).

### Suggesting enhancements

### Conventions for contributing

#### Programming in Julia

Julia is a programming language that is easy to learn and use. Their marketing slogan is *"Looks like Python, runs like C++"*. See the [Julia documentation](https://julialang.org/) if you are not familiar with it. If you already know Python, you will find Julia pretty easy to learn, don't worry.

Code blocks are some notebook-like spaces for the vulgarisers to demonstrate the theorical aspects of one of the fields covered by the project. For example :

![image](/assets/images/notebook_example_contributing_md.png)


For this purpose, we will use the [Pluto.jl](https://plutojl.org/) package, which is a notebook interface for Julia. For each notebook, you must export it to static HTML and put it in the [assets/notebooks](numenichal\assets\notebooks) folder. Then, at the place you want to display it on the website, you must use the following code:

```html
<iframe src="/numenichal/assets/notebooks/your_notebook.html"
        width="100%"
        height="600px"
        frameborder="0">
</iframe>
```

It will allow the website to display the notebook in an interactive way : users can run the code and see the outputs. On the image above, the notebook is just a screen capture because GitHub doesn't allow the iframe tag. But on the website, it will be interactive.

Note that the users can run the code or use it locally, so please make sure that the code is correct.

#### Latex

The following notations must be used in the website everytime we need to display some latex code : 

|notation|meaning|
|---|---|
|$\boldsymbol{x}$ (**bold** symbol)|2D or 3D vector|
|$x$ (normal symbol)|scalar|
|$\boldsymbol{M}$ (**bold** capital symbol)|order $2$ tensor of $ℝ^n$, with $n=2$ or $3$|
|$\{u\}$ (symbol between braces)|nodal values vector|
|$[M]$ (symbol between brackets)|finite element matrix|
|$f_{,i}$ (subscript under a function)|for multivariable functions, the partial derivative with respect to the $i$-th variable, equivalent to $\partial f/\partial x_i$|
|$a_ib_i$ (by abuse of notation) or $a_ib^i$ (correct tensorial notation)|Einstein notation for sums over repeated indices. For example, $a_ib_i$ means $\sum_{i=1}^n a_i b_i$, where $n$ is the dimension of the vector space.

Of course, usual conventions can override these ones, for example in the case of the stress tensor, which is usually denoted by $\boldsymbol{\sigma}$ and not $\boldsymbol{\Sigma}$. These conventions are just here to help all the contributors to be homogeneous for the benefits of the readers.
