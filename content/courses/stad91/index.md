---
title: "STAD91 Winter 2026 - Bayesian Statistical Inference"
date: 2026-01-05
lastmod: 2026-01-05
#aliases: 
#    - /courses/stad91/slides4.pdf
#    - /courses/stad91/slides1.pdf
#    - /courses/stad91/slides3.pdf
#    - /courses/stad91/slides2.pdf
#    - /courses/stad91/notes3.pdf
#    - /courses/stad91/notes4.pdf
#    - /courses/stad91/ps3.pdf
#    - /courses/stad91/ps4.pdf
#    - /courses/sta414/quiz1.pdf
#    - /courses/sta414/quiz2.pdf
#    - /courses/stad91/quiz3.pdf
#    - /courses/stad91/quiz4.pdf
#    - /courses/sta414/ps1.pdf
tags: ["Decision Theory", "Priors", "Posteriors", "Bayesian tests", "Model selection", "Sampling Algorithms", "Variational Bayes",
       "Asymptotics", "Gaussian Processes", "High-dimensional models", "Dirichlet process"]
author: "Thibault Randrianarisoa"
description: "This undergraduate/graduate course presents some modern techniques for probabilistic machine learning." 
summary: "The language of probability allows us to coherently and automatically account for uncertainty. This course will teach you how to build, fit, and do inference in probabilistic models. These models let us generate novel images and text, find meaningful latent representations of data, take advantage of large unlabeled datasets, and even let us do analogical reasoning automatically. It will offer a broad view of model-building and optimization techniques that are based on probabilistic building blocks which will serve as a foundation for more advanced machine learning courses." 
cover:
    image: "stad91.png"
    alt: "PML"
    relative: false
#editPost:
#    URL: "https://thibaultrandrianarisoa.netlify.app/courses/sta414/"
#    Text: "Course portal"
showToc: true
disableAnchoredHeadings: false

---

![Alt text](stad91.png)

## Introduction

This course introduces the core concepts of Bayesian statistics, the theoretical properties of Bayesian estimators and 
their use in decision-making under uncertainty. You will learn key Bayesian modelling approaches and advanced computational
techniques tailored to the needs  and structure of different models.

We begin with parametric models to introduce the core ideas of Bayesian analysis, covering prior specification, inference
(point estimation, credible sets, and hypothesis testing), its decision-theoretic foundations, and key asymptotic results
such as posterior consistency and the Bernstein–von Mises theorem. We will also study modern computational methods for
Bayesian inference and introduce more advanced topics, including high-dimensional and nonparametric models. For these models,
we will focus primarily on prior construction and on results about convergence rates and adaptation.

More details can be found in [syllabus](STAD91H3S-2026_Winter_Syllabus-20260105.pdf), [quercus](https://q.utoronto.ca/courses/429453) and 
[piazza](https://piazza.com/utoronto.ca/winter2026/stad91h3)
(Access Code: n0px27jcbmb).


[//]: # (## Outcomes)

[//]: # ()
[//]: # (- What you will learn:)

[//]: # (  * Standard statistical learning algorithms: When to use them, and their limitations.)

[//]: # (  * The main elements of probabilistic models: Distributions, expectations, latent variables, neural networks, and how to combine them.)

[//]: # (  * Standard computational tools: Monte Carlo, Stochastic optimization, Variational Inference, and automatic differentiation.)

[//]: # ()
[//]: # (- Skill Outcomes:)

[//]: # (  * Research Stream:)

[//]: # (    - Students will be able to mathematically derive custom model architectures and extend existing frameworks to handle different data structures.)

[//]: # (    - Identify when exact inference is feasible versus when approximate methods are required based on the characteristics of the model.)

[//]: # ()
[//]: # (  * Applied Stream:)

[//]: # (    - Evaluate the "cost of entry" for a project by estimating how much data and compute are required to reach target performance.)

[//]: # (    - Apply the "Linear-to-Complex" modeling workflow, starting with simple baselines to justify the use of more resource-intensive nonlinear models.)

## Announcements

+ [Practice midterm](Midterm.pdf) is out! Solutions will follow soon.
+ Lectures begin on Jan 8!

## Instructor

- Thibault Randrianarisoa, Office: IA 4064
  - Email: t.randrianarisoa@utoronto.ca (put “STA414” in the subject)
  - Office hours: Thursday 10am–1pm

## Teaching Assistants

Hanlong Chen (sl.chen@mail.utoronto.ca)

* He will handle all questions related to the practice final exam.

## Time & Location

Thursday, 3:00 PM - 6:00 PM

In Person: IA 1160

## Suggested Reading

The course will be based on some of the content of the book _Bayesian Data Analysis_ (BDA) by
Gelman, Carlin, Stern, Dunson, Vehtari & Rubin. It is freely available online on home page for
the book https://sites.stat.columbia.edu/gelman/book/, which also contains additional material
(lecture notes, code demo,...).

Additional suggested readings are:

* (TBC) Christian P. Robert (2007) [The Bayesian Choice](https://errorstatistics.com/wp-content/uploads/2016/03/robert-20071.pdf)
* (MCSM) Christian P. Robert and George Casella (2004) [Monte Carlo Statistical Methods](https://www.inference.org.uk/mackay/itila/book.html)
* (BC) Jean-Michel Marin and Christian P. Robert. (2007), [Bayesian Core : A Practical Approach to Computational Bayesian Statistics](https://link.springer.com/book/10.1007/978-0-387-38983-7)

## Lectures and (tentative) timeline

| Week                                         | Lectures                                                                                                                                                                                                           | Suggested reading                                | Problems                                                    | Timeline              |
|:---------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------|:------------------------------------------------------------|:----------------------|
| Week 1 <br/>5-11 January<br/>                | [Introduction and reminders of Statistics and Probability](BS_Lec01.pdf) <br/> <br/> [Annotated slides](BS_Lec01_annotated.pdf)                                                                                    | Sec. 1.2, 1.3, 1.8  (+ Appendix A for reminders) | [Sheet 1](PS1.pdf)  <br/> [Solutions](PS1sol.pdf)           |                       | 
| Week 2 <br/>12-18 January<br/>               | [Choice of priors, Aspects of the posterior](BS_Lec02.pdf)     <br/>  <br/>   [Annotated slides](BS_Lec02_annotated.pdf)                                                                                           | Sec. 1.5, 2.1, 2.4, 2.5, 2.8                     | [Sheet 2](PS2.pdf)  <br/>      [Solutions](PS2sol.pdf)      | [Quizz 1](Quizz1.pdf) | 
| Week 3 <br/>19-25 January<br/>               | [Decision theory](BS_Lec03.pdf)  <br/>  <br/>    [Annotated slides](BS_Lec03_annotated.pdf)     <br/>  <br/>     [Erratum](Erratum.pdf)                                                                            | Sec. 9.1                                         | [Sheet 3](PS3.pdf)        <br/>    [Solutions](PS3_sol.pdf) | [Quizz 2](Quizz2.pdf) | 
| Week 4 <br/>26 January-1 February<br/>       | [Bayesian tests, Model selection](BS_Lec04.pdf)                                                                                                                                                                    |                                                  | [Sheet 4](PS4.pdf)      <br/>    [Solutions](PS4_sol.pdf)   | [Quizz 3](Quizz3.pdf) | 
| Week 5 <br/>2–8 February<br/>                | Sampling Algorithms                                                                                                                                                                                                |                                                  |                                                             |                       | 
| Week 6 <br/>9–15 February<br/>               | Variational Bayes                                                                                                                                                                                                  |                                                  |                                                             |                       | 
| Week 7 <br/>16-22 February<br/>              | **Reading Week**                                                                                                                                                                                                   |                                                  |                                                             |                       | 
| Week 8 <br/>23 February – 1 March<br/>       | **Midterm**                                                                                                                                                                                                        |                                                  |                                                             |                       | 
| Week 9 <br/>2–8 March<br/>                   | Asymptotic properties in parametric Bayesian models                                                                                                                                                                |                                                  |                                                             |                       | 
| Week 10<br/>9–15 March<br/>                  | Priors for high-dimensional models                                                                                                                                                                                 |                                                  |                                                             |                       | 
| Week 11 <br/>16–22 March<br/>                | Dirichlet process                                                                                                                                                                                                  |                                                  |                                                             |                       | 
| Week 12 <br/>23–29 March <br/>               | Gaussian processes                                                                                                                                                                                                 |                                                  |                                                             |                       | 
| Week 13 <br/>30 March - 5 April<br/>         | Asymptotics in Bayesian nonparametrics                                                                                                                                                                             |                                                  |                                                             |                       | 

## Homeworks

| Homework #       | Out  | Due | TA Office Hours | Solutions |
|:-----------------|:-----| :--- | :--- | :--- |
| **Assignment 1** | TBD  | TBD  | TBD  |  |
| **Assignment 2** | TBD  | TBD  | TBD  |  |


## Computing Resources

For the homework assignments, we will primarily use Python, and libraries such as [NumPy](https://numpy.org/), 
[SciPy](https://scipy.org/), and [scikit-learn](https://scikit-learn.org/stable/). You have two options:

* The easiest option is run everything on [Google Colab](https://colab.research.google.com/).
* Alternatively, you can install everything yourself on your own machine.
    - If you don’t already have python, install using [Anaconda](https://www.anaconda.com/download).
    - Use pip to install the required packages `pip install scipy numpy autograd matplotlib jupyter sklearn`
* For those unfamiliar with Numpy, there are many good resources, e.g. [Numpy tutorial](https://realpython.com/numpy-tutorial/) 
and [Numpy Quickstart](https://numpy.org/doc/stable/user/quickstart.html).

