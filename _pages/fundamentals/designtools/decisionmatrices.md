---
permalink: /fundamentals/designtools/decisionmatrices/
title: "Decision Matrices"
layout: single
sidebar:
    nav: "fundamentals"
    
---

When you are first conceptualizing your UAV, one of the first things you will do is determine a configuration. One way of doing this is to use a decision matrix, or *Pugh matrix*. Strategies on how to do this effectively will be discussed here.

## Selecting Configurations
Before using the Pugh matrix, you will need to select a few different [configurations](https://aeronautics.byu.edu/fundamentals/aerodynamics/configurations/). These may have a few features in common or be completely different. In any case, you will want to pick 2-4 different configurations that fit well with the [mission requirements](https://aeronautics.byu.edu/fundamentals/designtools/definingrequirements/) that you have already determined. One way of visualizing your configurations is to use a program like [OpenVSP](http://openvsp.org/) to create a quick CAD model (see Figure 1). Once you have a few selected, they can be compared in the Pugh matrix.

{% include figure image_path="_pages/fundamentals/designtools/figures/VSP_Model_1.PNG" caption="Figure 1: A simple model produced with OpenVSP." %}

## The Pugh Matrix
Since this is just the conceptual stage of the design process, most of the design decisions are more qualitative than quantitative. The Pugh matrix is essentially a way of putting figures to help make those decisions. We can use the Pugh matrix here to compare three different configurations using a series of metrics. These should be what you believe are the most important considerations for your mission. It is common to weight each metric based on its relative importance. The table below depicts an example with three different configurations being compared.

| Metric                 | Option 1 | Option 2 | Option 3 | 
| ---------------------- | -------- | -------- | -------- | 
| Stability (x3)         | 3        | 2        | 1        | 
| Complexity (x2)        | 1        | 3        | 3        | 
| Drag (x3)              | 2        | 3        | 3        | 
| Coolness (x1)          | 3        | 1        | 3        | 
| Durability (x2)        | 2        | 2        | 1        | 
| Manufacturability (x2) | 1        | 2        | 1        | 
| **Total**              | **26**   | **30**   | **25**   | 

Another way of doing this is to compare individual parameters of the UAV rather than entire configurations. As an example, we will only compare a few parameters for the main wing. You can see the results in the table below.

| Metric                 | Taper  | No Taper | Large AR | Small AR | Swept  | Unswept |
| ---------------------- | ------ | -------- | -------- | -------- | ------ | ------- | 
| Stability (x3)         | 3      | 2        | 3        | 3        | 2      | 3       | 
| Complexity (x2)        | 2      | 3        | 3        | 3        | 2      | 2       | 
| Drag (x3)              | 2      | 1        | 1        | 3        | 2      | 2       | 
| Coolness (x1)          | 3      | 1        | 2        | 1        | 3      | 2       | 
| Durability (x2)        | 2      | 2        | 2        | 3        | 3      | 2       | 
| Manufacturability (x2) | 2      | 3        | 2        | 3        | 1      | 3       | 
| **Total**              | **30** | **26**   | **28**   | **37**   | **29** | **31**  | 

Using a Pugh matrix should inform your final configuration decision, but there may be other considerations that can't be measured such as availability of materials, team member skill limitations, and so forth. In any case, it can be a tremendous tool during the vital early stages of your design project.
