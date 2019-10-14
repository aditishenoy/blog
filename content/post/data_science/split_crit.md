---
title: "How do I split my data?"
date: 2019-08-24T19:40:37+05:30
draft: false
image: 
tags: ["Data Science"]
categories: ["blog"]
---

This post will describe various dataset splitting strategies for machine learning problems. We will start by looking at why we need to think about different splitting approaches i.e. considering the 'Bias-Variance tradeoff', the current methods used and recent methods for splitting depending on the nature of the problem. 

 The outline of the post is as follows: 

1. Understanding bias-variance tradeoff
2. Previous ways of splitting data 
3. Modern ways of splitting 
4. Things to take into consideration while defining the split 


Ensuring model generalizability as well as learning (Bias vs Variance Dilemma)

B) Earlier ways of splitting data - small data sets 

using 70/30 or 80/20 or 60/20/20

For eg. 





Modern machine learning - million training samples training - 98 and D/T as 1/1

test set helps to evaluate how good the system is - big enough for high confidence in overall performance 

C) Cross validation (hold-out crossvalidation (early stopping) and k-fold cross-validation)

1) Random sampling (row-wise)
stratified random sample based on the outcome
> Randomly by rows - rows independent by eachother 

Completely random sampling is a straightforward strategy to implement and usually protects the process from being biased towards any characteristic of the data. 

The data in the validation and testing dataset should have the same distribution.

To partition the data, the splitting of the orignal data set will be done in a stratified manner by making random splits in each of the outcome classes.

 we can implement the split by randomly sampling connected components, instead of randomly sampling rows
 

Using R: 

* Simple Splitting Based on the Outcome: 
function createDataPartition can be used to create balanced splits of the data.

* Splitting based on dissimilarity among predictors 

* Splitting for time-dependent data 

Timewise (everything before date training, and after is testing) - moving window validation 

rolling forecasting origin techniques that move the training and test sets in time


3) Based on Unique ID

4) Combinations 




Logic of feature generation depends on data splitting strategy; important to mimic the train/val split same as train/test split 



### References: 

* https://bookdown.org/max/FES/splitting.html
* https://topepo.github.io/caret/data-splitting.html#simple-splitting-based-on-the-outcome
