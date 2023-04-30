Download Link: https://assignmentchef.com/product/solved-ics-assignment-2-modelling-the-spread-of-cvoid-19
<br>
5/5 - (1 vote)




In this assignment we will be exploring other ways to model infectious diseases. In the first part of the assignment we will use a stochastic discrete event model to compute the spread of an infectious disease through a population. And in the second half of the assignment we will explore spatial models to study the spread of infectious diseases.

Problem 1: Gillespie’s Direct Algorithm

We have discussed the five hallmarks of stochastic SIR dynamics: variability; negative co-variances; increased transients; stochastic resonance; and extinctions. Some of those were demonstrated in the stochastic versions of the SIR ODEs (using constant or scaled noise terms) and some were shown in the context of event driven SIR.

We ask you to explore the five hallmarks in an SIR discrete event model using Gillespie’s direct algorithm. Design a set of well chosen experiments to demonstrate all these as- pects,also exploring the dependence on the basic parameters in the model.Advanced topic: Try to reproduce the graphs from the book in relation to persistence and critical community size, or try to measure e.g. the first passage time. You can also consider other models, e.g. SIS, SEIR, SIRS, etc.

Hint: start with SIR without demography, then add demography, and finally add imports to the model.

Problem 2: Spatial Models

1. Meta-population model: Lets start with implementing a simple meta-population model to study the spatial dynamics of a spreading infection. Start with a stochastic meta-population model with two sub-populations. Consider two large, fully suscep- tible populations, with ρii = 1 and ρij &lt; 1. Assume the populations are of the same size, and ignore demography. What is the effect of the coupling between the two populations, are there any delays?

Now produce a meta-population of your own using more sub populations (Hint: Try using different strength of interaction between populations), and comment on the dynamics.

2. Network model and Vaccines: In this question you are asked to develop a set of experiments to design and evaluate vaccination strategies using a network model. Using the package NDLib1 you should assess the spread of a disease (SIR) across

1Note there are SIR Network implementations/examples that you can re-use/adapt in the library see https://ndlib.readthedocs.io/en/latest/tutorial.html

Introduction to Computational Science Assignment 2

different types of networks (Barabasi Albert, Watts-Strogatz, Erdos-Reyni). You can consider:

<ol>

 <li>(a)  How to assess the impact/spread of the epidemic (what to measure).</li>

 <li>(b)  How to vary disease initalisation – how many and which nodes to start the infection with.</li>

 <li>(c)  Design and evaluate a vaccine strategy and test its effectiveness on the different networks. This vaccine strategy should decide which nodes to vaccinate – you might consider strategies where you know the network structure OR strategies where you don’t have global network information (i.e., deliver at random).</li>

</ol>