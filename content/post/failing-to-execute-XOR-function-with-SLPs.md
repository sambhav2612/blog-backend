---
title: "Failing to compute XOR-functions with an SLP"
date: 2018-06-06T23:14:11+05:30
draft: false
tags: ["ai", "ml", "deep learning", "blog"]
categories: ["starting", "blog", "research", "deep learning"]
comments: true
toc: true
formspree: true
---

**NOTE**: More content would be added later with appropraite images for enhanced understanding of the topic.

# Background

For some time now, I was wondering to get started with researching deep learning as a domain on my own. So, I waited till my semester exams passed and summer vacations came around. Since, I didn't sent any patch to this year's GSoC Orgs I was unable to become a part of the GSoC Clan. Nevertheless, I like researching, finding issues, harnessing powers of the Internet knocking at my doorstep to point in the direction of growth, which is like what **Mars is to Elon Musk**.

# Foreground

At my last dev meetup with regional GDG group, we were inducted with Deep Learning Models. I prefer unsupervised models instead of supervised models due to their tendency to adapt from previous inputs.

### DL vs ML: An Engima

The core difference between Deep Learning and Machine Learning lies in how the procedures are carried out; in deep learning we determine the output by using a layered-heirarchical structure, a structure that evloves in terms of real-life reperesentation of features it describes after the previous layer. While in machine learning the procedure takes in examples hard-coded already by the developers to give some desired result. Machine Learning hence learns to adapt to find the solution through several similar examples of the problem it is going to adapt to solve on its own.

### Feature Hierarchy/Concept Tree

Now, the most trivial layer is called **Visible Layer**, which the what the visible input is sent to be classified by the deep learning algorithm. Each successive layer takes in the output of immediate previous layer as its own input and proceeds with more robust classification than before. These middle layers are called **Hidden Layers** which as the name suggests are hidden within the algorithm, not visible at input or output.

# Deeeep enough to crawl through?

> The word deep in deep learning comes from the depth (shortest length to traverse from the that node/element to the output layer, analogous to the heights in the tree data structure) of hierarchical-layered structure defined.

Deep Learning isn't something new either, first came **Cybernetics** in '40s and '50s followed by **Connectionsism** later in '80s then finally as **Deep Learning** in the 2006-ish timeline. However, these are just buzzwords and the reality is that what people were doing 70 years back are even doing now, because it can (and will) simulate a living-cognitive mind.

### A brief introduction to Perceptrons

McCulloch-Pitts (1943) gave an algorithm to train trivial deep learning models by artificical neurons called Perceptrons. A perceptron can only have binary output i.e., 0 or 1 hence was very suitable for solving boolean algebra. Nah, it wasn't as much advance as they had thought but it is marvel of study in deep learning. Here, I'd write about how and why it failed to compute the XOR-function.

### Single-layered

An SLP (**S**ingle **L**ayer **P**erceptron) has only two layers, one input layer and one output layer hence the input comes and goes just after the trivial classification from the visible layer while input is taken. This means that an SLP only works for a single line of input-output.

### Multi-layered

On thr other hand a multi-layer perceptron has many intermediate layers in betweem input and output to figure out the desired output with more precision.

# The XOR-function

