---
layout: post
title:  "Some basic optimization algorithms in Python"
date:   2017-05-17
categories: optimization
---

After taking a convex optimization class this past semester I implemented a few basic algorithms for unconstrained optimization (e.g. [Nesterov's accelerated gradient descent](https://github.com/idc9/optimization_algos/blob/master/opt_algos/accelerated_gradient_descent.py)) in Python in this repo: [**https://github.com/idc9/optimization_algos**](https://github.com/idc9/optimization_algos).

The purpose of this repo is for me to learn and to have bare bones implementations of these algorithms sitting around. I tried to make the code modular and simple as possible so that you (or a future me) can modify it for other purposes (e.g. add bells and whistles, implement other algorithms, etc). While off the shelf solvers such as [sklean](http://scikit-learn.org/stable/) or [cvxopt](http://cvxopt.org/) are preferable for many applications there are times when you want full control over the solver.


Right now the repo focuses on first order methods (GD, SGD, accelerated GD, etc) for [empirical risk minimization](http://www.cs.cornell.edu/courses/cs4780/2015fa/web/lecturenotes/lecturenote10.html) problems. For some useful introductory references see:

- [An overview of gradient descent optimization algorithms](http://sebastianruder.com/optimizing-gradient-descent/index.html) by Sebastian Ruder (good high level overview)
- [Optimization Methods for Large-Scale Machine Learning](https://arxiv.org/abs/1606.04838) by Léon Bottou, Frank E. Curtis, and Jorge Nocedal
- [Convex Optimization](https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf) by Boyd and Vandenberghe (or see [video lectures](https://www.youtube.com/view_play_list?p=3940DD956CDF0622))

A few more interesting references:
- [Convex Optimization: Algorithms and Complexity](https://arxiv.org/pdf/1405.4980.pdf) by Sebastien Bubeck
- [Nesterov's Accelerated Gradient Descent for Smooth and Strongly Convex Optimization](https://blogs.princeton.edu/imabandit/2014/03/06/nesterovs-accelerated-gradient-descent-for-smooth-and-strongly-convex-optimization/)
- [Why Momentum Really Works](http://distill.pub/2017/momentum/)
