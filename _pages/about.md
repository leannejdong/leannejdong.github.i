---
permalink: /
title: "Research Spotlight"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I am a Mathematician and a freelance software engineer. Currently I work in the Fintech domain
for open source software development. Last year, I built an asynchronous software development kit library [sdk](https://github.com/bitwyre/sdk/tree/develop/cpp/source) to the RESTful API for financial trading. Currently I'm building trading bots (both sync, async) based on my developed SDK.

I have a wide range of interests, from hard core engineering, architectural design of software, backend to frontend development. Currently I'm open for interesting software collaborations.

Formerly (between 2020-2022) I was an industry postdoc researcher working  @ [Concordia University, School of Engineering and Computer Science](https://www.concordia.ca/ginacody.html). My advisors are
[Ursula Eicker](https://www.concordia.ca/next-gen/eicker.html), [Jia Yu Yuan](https://users.encs.concordia.ca/~jiayuan/) and [Freddy Lecue](http://www-sop.inria.fr/members/Freddy.Lecue/).


At my postdoc, I developed an undirected graph concept for hydraulic-thermal network, extension of a DSL compiler for renewable energy and a CLI application for multiway sparse decison tree optimization. At my first postdoc, I worked on computer social media. I built dependence structure between labor occupation based on job counts data,  using copulae. I also developed a theoretical model based on hawkes intensity point processes allows fitting information diffusion based on observed counts of events. The main tools we used were functional analysis and distribution theory. I completed my [PhD](https://www.maths.usyd.edu.au/ut/people?who=LJ_Dong) in early 2018 on the topic of stochastic Navier-Stokes equations on the rotating spheres with stable Lévy noise, under supervision of Prof. Beniamin Goldys, the univeristy of Sydney. I have been teaching in universities on various topics for roughly 10 years. Prior to my PhD, I was a researcher in quantitative finance and stochastic processes.

Two main themes of my last postdoc research were:

**District Heating and Electricity Networks**

* Extend the [INSEL(integrated simulation environment language)](https://www.insel.eu/en/) compiler functionality to sort the model of an undirected graph, that is, the order the nodes and edges represented by blocks
identified by their block numbers;

* Build network graph topology.

* Undirected Graph Parser

* Loop detections 

* Automate system of equations

* Generic solver for Nonlinear Networks

* Integration of network simulation solver to the Urban Modelling Platform 

**Theorectical and Interpretable Machine Learning**

Decision trees have been a popular Machine Learning model dates back to the 90s due to its interpretability. One starts with a simple tree, keep branching out
to improve its accuracy. Stopping conditions are applied to  avoid overfitting. The problem of this approach is, if we chose the wrong split at the beginning, there is no way
to un-do it. Historically, mathematical optimization solvers have been used to circumvent overfitting. However, in order to fully optimize the decision trees, one has to step through 
a search space both in theory and practice hard.(Full optimality of decison tree has been well-known as a NP-hard problem)
I follow a specialized algorithm developed in [GOSDT](https://arxiv.org/abs/2006.08690) that combines dynamic programming and branch and bound to optimize a generalize objective.
The objective function consists of a sparsity term that penalize the number of leaves in the tree. The resulting trees depend on the choice of loss functions.
Here are a few features of the GOSDT algorithms

* Analytical bounds. The collection of bounds allow us to skip over a large portion of the search space

* Dynamic programming. Split dataset into subsets until higher accuracy is achieved. The solution for one duplicated instance can be used for another.

* Dependency graph. The DP formulation creates a dependency graph between sets and subsets. Each set is responsible for finding optimal features to sub-divide itself into 
additional subsets. Each subset decides the best feature to split. Once enough subsets decided, the optimal tree will emerge as DAG of the best features.

* Priority queue. For scheduling problems.

The existing GOSDT algorithm works only for binary features, which may not be ideal for training data with multiple features. During part of my fellowship, I developed a C++ implememntation that converts the binary decision tree to n-ary tree decision tree with the existing parallelism. See [mgosdt](https://gitlab.com/leannejdong/mgosdt/-/tree/async) for C++ implementations.

**Topics of interests**: 

* Graph theory and algorithms

* C++ (Non-ancient) : Real-time low latency

* Scientific computing for partial differential equations

<!---

**Past Interests**

* Mathematical Analysis of Artificial Intelligence and Theoretical Computer Science

* Theoretical or Statistical Machine Learning

* Stochastic PDEs, Financial Mathematics

* Quantum Computing, Quantum game theory, Information Geometry, Quantum Machine Learning

* Point processes and applications to Social Media, Finance, Insurance, Quantum Physics

--->

