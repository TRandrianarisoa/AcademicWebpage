---
title: "STA414 / STA2104 Winter 2026 - Statistical Methods for Machine Learning II"
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
tags: ["Probabilistic Models", "DAGs", "Decision Theory", "Exact Inference", "Message Passing", "Hidden Markov Models",
  "Sampling Methods", "MCMC", "Variational Inference", "Neural Networks", "Gaussian Processes", "Embeddings",
  "Attention", "Transformers", "Variational Autoencoders", "Diffusion Models"]
author: "Thibault Randrianarisoa"
description: "This undergraduate/graduate course presents some modern techniques for probabilistic machine learning." 
summary: "The language of probability allows us to coherently and automatically account for uncertainty. This course will teach you how to build, fit, and do inference in probabilistic models. These models let us generate novel images and text, find meaningful latent representations of data, take advantage of large unlabeled datasets, and even let us do analogical reasoning automatically. It will offer a broad view of model-building and optimization techniques that are based on probabilistic building blocks which will serve as a foundation for more advanced machine learning courses." 
cover:
    image: "Sta414.png"
    alt: "PML"
    relative: false
#editPost:
#    URL: "https://thibaultrandrianarisoa.netlify.app/courses/sta414/"
#    Text: "Course portal"
showToc: true
disableAnchoredHeadings: false

---

![Alt text](Sta414.png)

## Introduction

The language of probability allows us to coherently and automatically account for uncertainty. This course will teach 
you how to build, fit, and do inference in probabilistic models. These models let us generate novel images and text, find
meaningful latent representations of data, take advantage of large unlabeled datasets, and even let us do analogical 
reasoning automatically. It will offer a broad view of model-building and optimization techniques that are based on 
probabilistic building blocks which will serve as a foundation for more advanced machine learning courses.

More details can be found in [syllabus](), [quercus]() and [piazza](https://piazza.com/utoronto.ca/winter2026/stad91h3)
(Access Code: n0px27jcbmb).


## Outcomes

- What you will learn:
  * Standard statistical learning algorithms: When to use them, and their limitations.
  * The main elements of probabilistic models: Distributions, expectations, latent variables, neural networks, and how to combine them.
  * Standard computational tools: Monte Carlo, Stochastic optimization, Variational Inference, and automatic differentiation.

- Skill Outcomes:
  * Research Stream:
    - Students will be able to mathematically derive custom model architectures and extend existing frameworks to handle different data structures.
    - Identify when exact inference is feasible versus when approximate methods are required based on the characteristics of the model.

  * Applied Stream:
    - Evaluate the "cost of entry" for a project by estimating how much data and compute are required to reach target performance.
    - Apply the "Linear-to-Complex" modeling workflow, starting with simple baselines to justify the use of more resource-intensive nonlinear models.

## Announcements

+ Lectures begin on Jan 6!

## Instructor

- Thibault Randrianarisoa, Office: UY 9179
  - Email: t.randrianarisoa@utoronto.ca (put “STA414” in the subject)
  - Office hours: Tuesday 9:30-11:30

## Teaching Assistants
Yichen Ji, Shengzhuo Li, Liam Welsh, Yan Zhang, Amir Reza Peimani

* They will handle all questions related to homework assigments, the midterm and the final exam.
* Email: TBA (in the subject of the email indicate the scope: HW1, HW2, general, etc)

## Time & Location

Tuesday, 6:00 PM - 9:00 PM

In Person: MC 102

## Suggested Reading

No required textbooks. Some suggested readings are:

* (PRML) Christopher M. Bishop (2006) [Pattern Recognition and Machine Learning](https://www.microsoft.com/en-us/research/people/cmbishop/prml-book/)
* (DL) Ian Goodfellow, Yoshua Bengio and Aaron Courville (2016), [Deep Learning](https://www.deeplearningbook.org/)
* (MLPP) Kevin P. Murphy (2013), [Machine Learning: A Probabilistic Perspective](https://probml.github.io/pml-book/book0.html)
* (ESL) Trevor Hastie, Robert Tibshirani, Jerome Friedman (2009) [The Elements of Statistical Learning](https://hastie.su.domains/ElemStatLearn/)
* (ISL) Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani (2023) [Introduction to Statistical Learning](https://www.statlearning.com/)
* (ITIL) David MacKay (2003) [Information Theory, Inference, and Learning Algorithms](https://www.inference.org.uk/mackay/itila/book.html)
* (PML1) Kevin P. Murphy (2022), [Probabilistic Machine Learning: An Introduction](https://probml.github.io/pml-book/book1.html)
* (PML2) Kevin P. Murphy (2023), [Probabilistic Machine Learning: Advanced topics](https://probml.github.io/pml-book/book2.html)


## Lectures and (tentative) timeline

| Week                                   | Lectures                                    | Suggested reading | Tutorials | Video | Timeline |
|:---------------------------------------|:--------------------------------------------|:------------------|:----------| :--- | :--- |
| Week 1 <br/>5-11 January<br/>          | Introduction / Probabilistic Models         | PML1 1.1-1.3      |           | | |
| Week 2 <br/>12-18 January<br/>         | Directed Graphical Models / Decision theory |                   |           | | |
| Week 3 <br/>19-25 January<br/>         | Exact inference / Message Passing           |                   |           | | |
| Week 4 <br/>26 January-1 February<br/> | Hidden Markov Models / Monte-carlo Methods  |                   |           | | |
| Week 5 <br/>2–8 February<br/>          | MCMC                                        |                   |           | | |
| Week 6 <br/>9–15 February<br/>         | Variational Inference                       |                   |           | | |
| Week 7 <br/>16-22 February<br/>        | **Reading Week**                            |                   |           | | |
| Week 8 <br/>23 February – 1 March<br/> | **Midterm**                                 |                   |           | | |
| Week 9 <br/>2–8 March<br/>             | Neural Networks                             |                   |           | | |
| Week 10<br/>9–15 March<br/>            | Gaussian Processes                          |                   |           | | |
| Week 11 <br/>16–22 March<br/>          | Embeddings/Attention/Transformers           |                   |           | | |
| Week 12 <br/>23–29 March Janurary<br/> | Variational Autoencoders                    |                   |           | | |
| Week 13 <br/>5-11 Janurary<br/>        | Diffusion Models                            |                   |           | | |

## Homeworks

| Homework #       | Out  | Due | TA Office Hours | Solutions |
|:-----------------|:-----| :--- | :--- | :--- |
| **Assignment 1** | TBD  | TBD  | TBD  |  |
| **Assignment 2** | TBD  | TBD  | TBD  |  |
| **Assignment 3** | TBD  | TBD  | TBD  |  |
| **Assignment 4** | TBD  | TBD  | TBD |  |

## Computing Resources

For the homework assignments, we will primarily use Python, and libraries such as [NumPy](https://numpy.org/), 
[SciPy](https://scipy.org/), and [scikit-learn](https://scikit-learn.org/stable/). You have two options:

* The easiest option is run everything on [Google Colab](https://colab.research.google.com/).
* Alternatively, you can install everything yourself on your own machine.
    - If you don’t already have python, install using [Anaconda](https://www.anaconda.com/download).
    - Use pip to install the required packages `pip install scipy numpy autograd matplotlib jupyter sklearn`
* For those unfamiliar with Numpy, there are many good resources, e.g. [Numpy tutorial](https://realpython.com/numpy-tutorial/) 
and [Numpy Quickstart](https://numpy.org/doc/stable/user/quickstart.html).

