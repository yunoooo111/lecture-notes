---
title: "polynomial integration"
date: 2023-08-24T17:39:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi4002']
draft: false
math: true
url: "0018"
---
Polynomial is sum of terms, which is built with constant, variables, and exponent ([Pierce, 2021](https://www.mathsisfun.com/algebra/polynomials.html)),  where the exponent is greater and equal to zero ([Gruber & user103828, 2015](https://math.stackexchange.com/a/321264/645927)). Then integral of any polynomial is simply sum of the integrals of its tems, whose formula of its indefinite integral is well known ([Nave, 2017](http://hyperphysics.phy-astr.gsu.edu/hbase/intpol.html)) and its definite integral can be calculated  with the help of the formula, e.g. using Python ([Mehta, 2021](https://www.geeksforgeeks.org/integration-in-a-polynomial-for-a-given-value/)). Simpson's rule can calculate integral of polynomial function by approxymating it with set of quadratic functions ([Kong et al., 2020](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter21.04-Simpsons-Rule.html)), but not recommended since it is not very efficient compared to the use of its indefinite integral formula.
