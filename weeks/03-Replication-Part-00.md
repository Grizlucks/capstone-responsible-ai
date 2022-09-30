---
layout: week
title: Week 03
permalink: /weeks/03-Replication-Part-00/
doodle: /doodle.png
---

# Replication Project Part 0: Introduction

## Topics

This week's assignments will guide you through the following topics:
* Think about what Malware is, and how you identify it in source code.
* Build a data processing pipeline to extract features from smali.

## Reading

Please read the following:
* Read the
  [HinDroid](https://www.cse.ust.hk/~yqsong/papers/2017-KDD-HINDROID.pdf)
  paper through section 3.1 (feature extraction). Read this
  thoroughly!
* For more information on the structure of APKs and Android Bytecode
  (e.g. Smali), read section II of this
  [paper](https://arxiv.org/pdf/1808.04218.pdf).

## Tasks

**Note:** These tasks will be difficult, and potential take awhile to
compute, so start early!

Complete the following tasks:

* Write parsing code for the test files in
  `/teams/DSC180A_FA20_A00/a04malware/test-apps` on the server. Your
  code should extract all the information needed to create the
  matrices `A`, `B`, `P`, `I` in the Hindroid paper and put that
  information in a csv file. My suggestion would be to have each
  observation in the csv correspond to an api call found in one of the
  classes/files. How exactly you organize it is up to you, though!
* Calculate the distribution/counts of APIs, packages,
  package-families (`L<family>/`), and invoke-types in each app. How
  many distinct shared apis do each pair of apps have? distinct
  packages? 
* Build the adjacency matrix A for the given test apps.


## Weekly Questions

Answer the following questions on Canvas:

* How many distinct APIs occur in the Instagram App?
* What are the dimensions of A for the test apps?
* For each adjacency matrix A, B, P, interpret in plain english how
  two elements connected by an edge should be considered
  *similar*. How will these similarities help us identify malware?
