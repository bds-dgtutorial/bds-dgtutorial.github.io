---
title: DG Tutorial
feature_text: |
  ## A Short Tutorial on Domain Generalization
  This tutorial serves as a starting point for researching the field.

  9:00-9:55 am, Monday, July 17th, Athens, Greece
feature_image: "/assets/images/background.jpg"
excerpt: "Rather than starting from scratch, this tutorial is designed to help individuals navigate the DG literature."
---

Rather than starting from scratch, this tutorial is designed to introduce anyone interested to the problem of Domain Generalization
and assist whoever wants to get into the field navigate the literature.

{% include button.html text="Slides 🔗" link="/assets/dg_tutorial_slides.pdf" color="#0366d6" %} 

## Introduction

Domain Generalization is a fundamental problem in
machine learning today. Despite the fact that
deep learning models have seen immense success in
the past few years even surpassing experts in some
cases they often fail to mimic the adaptability
prowess of humans. The development of highly generalizable
and robust ML models proves to be exceptionally difficult
in numerous cases, as the distribution shifts present across
separate datasets or databases cause a model’s performance
to deteriorate, or even completely break down, when
evaluated on previously unseen data.
Most ML models depend on the assumption that the test
samples are independent from and identically distributed (i.i.d.) with the training data. In practice, even though the independence assumption
commonly holds, the test data often follows
a different data generating distribution than the training data. This creates a need for the development of algorithms which are not affected 
by the distributional shift present in distinct data domains of the same problem - or in other words, *domain generalizable* models. 

This short tutorial serves as an introduction to the field of 
*Domain Generalization* and presents its most important aspects, from problem statement, to state-of-the-art methods and evaluation settings. 

## Presenters

- [Christos Diou](https://diou.github.io), Assistant Professor of Artificial Intelligence and Machine Learning, Harokopio University of Athens, cdiou@hua.gr
- [Aristotelis Ballas](https://aristotelisballas@github.io), PhD Student, Harokopio University of Athens

## Outline
1. Introduction to DG 
2. Overview of representative DG methods
3. DG datasets and benchmarks
4. DG for biomedical signals: The BioDG benchmark
5. Conclusions
6. Appendix

Below you may find a taxonomy of the domain generalization methods 
proposed in the literature.

![alt text](/assets/images/dgoutline.png) 

## BioDG: A Benchmark for Domain Generalization in Biosignal Classification

We introduce an open-source DG evaluation benchmark, namely
BioDG, for 12-lead ECG and 62-channel EEG biosignals. BioDG adapts 
SoTA DG algorithms from the image classification domain for 1D 
biosignal classification.  


![alt text](/assets/images/benchmark.png) 

We propose an alternative neural network architecture 
which leverages intermediate representations from multiple
layers of a CNN.

![alt text](/assets/images/biodg_model.png)

If you want to find out more about our work, please 
visit the following links:

{% include button.html text="Paper 🔗" link="https://arxiv.org/abs/2303.11338" color="#0366d6" %} {% include button.html text="Code" icon="github" link="https://github.com/aristotelisballas/biodg" color="#0366d6" %} 


## Acknowledgment
The work leading to these results has been funded by the European Union under Grant Agreements No. 101057821, project RELEVIUM and European Union’s Horizon 2020 research and innovation programme under Grant Agreement No. 965231, project REBECCA (REsearch on BrEast Cancer induced chronic conditions supported by Causal Analysis of multisource data).

<img src="/assets/images/relevium.png" alt="" width="100">
<img src="/assets/images/rebecca.png" alt="" width="100">
