# Neural_Network_Charity_Analysis
UCB-Data-19

## Overview

We trained a model on data from startup grant requests to predict the expected success of incoming requests. Our goal was a 75% prediction rate on the randomized test data, but unfortunately our best run topped out just under 73%. After running 30 to 40 different combinations of activation features, I settled on 3 approaches that got us within 3% of the target amount. Node count was toyed with a great deal as well, ended up on 2 hidden layers for a higher consistency in trial runs. 

## Preprocessing Process

* Target was pretty cut and dry. Was the company a success, regardless of funding received or aim.
* I cut out amount requested column as it isn't actually relevant in our dataset to success rate. Preliminary models with it included maxed out at a 53.21% accuracy, regardless of activations, node count, or layers.
* What columns were included were toyed with a fair bit. Including training a model on only yearly income, and another trained on only the application type. The predictive nature of these were subpar to including the whole dataset.

## the Model

* 28, 21, 14 neurons, 3 modules, and swish activation came out on top.'
* A stripped down neuron structure and a neuron structure that darn near overheated my system were attempted. There wasn't a meaningful amount of deviation, so I chose multiples of 7 for the heck of it.
* I was not able to achieve the target, but came within 1.9% during trial runs.
* Every aspect of the translation was altered in some way at some point to achieve the results. swish activation in particular was a game changer.

## Summary

While we were not successful in meeting the target goal of 75% and having done the due diligence to create 3 models with similar results and literally hundreds of configurations that resulted in lesser results, I have reached the conclusion that this is a project and model that is best served with more available data and more time spent on the project. With that said, I'm happy with the results as I gleaned a lot of information about the operations of different activation functions and different methods of compiling the data. 
