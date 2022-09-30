---
layout: week
title: Week 01
permalink: /weeks/05-AI-Regulations/
doodle: /doodle.png
---

# AI Regulations

## Topics

This week's assignments will guide you through the following topics:
* Finishing a baseline model
* Creating the HIN in the Hindroid paper

## Reading

Please read the following:
* (Re)Read
  [HinDroid](https://www.cse.ust.hk/~yqsong/papers/2017-KDD-HINDROID.pdf)
  section 3.2, along with section 4-4.2. You will have to read section
  3.2 _many_ times!
* Review SVMs and the "Kernel Trick" (The *communiting matrices* of
  section 3.2 will be the kernel in our SVM classifier).

## Tasks

Complete the following tasks:
* Finish you work from last week: create a baseline model using
  hand-coded features developed in the previous two weeks. Create a
  few new features this week (e.g. derived from the Package or method
  name for example, informed by your EDA). The choice of classifier is
  up to you. (Note: you should *not* be implementing Hindroid
  here). What is the most appropriate *evaluation metric* here? (Hint:
  it's not accuracy).
* Implement the commuting matrix `AA^T` (keep in mind you will have to
  do this commuting matrices involving `B`, `P`, and `I` next week as well!). That
  is, write code that takes your intermediate csv data and creates the
  commuting matrix `AA^T` in Hindroid.
* Take one of the Malware types you investigated this week and find
  the code in smali where the 'bad' behavior occurs (if you cannot
  solve this, it's ok).
  
*Note 1:* Not all of the APIs in the dataset may be needed to compute
commuting matrices. Which apis might you be able to ignore (think
about what `AA^T` is -- and how it measures similarity between two
apps).

*Note 2:* You may find [sparse
matrices](https://docs.scipy.org/doc/scipy/reference/sparse.html)
valuable. Explore the documentation and share useful tutorials on
slack (e.g. [this
one?](https://machinelearningmastery.com/sparse-matrices-for-machine-learning/)).


## Weekly Questions

Answer the following questions on Canvas:
* Consider the commuting matrix `AA^T` in the Hindroid paper. What do
  the elements represent?
  - Give an answer in terms of paths on hindroid's HIN (graph).
  - Give an answer that is generally understandable, in iterms of
    `app`s and `api`s.
* What evaluation metric(s) for your baseline did you use and why?
* What was the most difficult thing you experienced this week, to
  discuss in section.
