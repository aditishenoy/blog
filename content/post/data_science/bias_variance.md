---
title: "What is Bias, Variance and Bias-Variance Tradeoff?"
date: 2019-08-24T10:31:26+05:30
draft: false
tags: ["Data Science"]
categories:
image: '/img/highlighter.jpg'
comments: true
share: true
---

<!--Welcome to Part 1 of 2 of blog posts talking about Bias-Variance Tradeoff and different criteria and strategies for splitting datasets for training and testing. The second part of this series discussing data splitting approaches can be found [here]().-->

This blog post will talk about bias, variance and why it is important to consider the tradeoff between these parameters as well as model complexity while choosing machine learning algorithms for the problem we are trying to solve. 

## Bias

The objective of any supervised machine learning algorithm is to predict an outcome (target) using input data (features) on data that the model hasn't ever seen before. In order to do this, the model makes some assumptions to simplify the problem and find patterns to learn the data. This is called 'bias'. It is referred to as the difference between average prediction and the correct value. Algorithms which make fewer assumptions while training have low bias e.g. Support Vector Machines (SVM), kNN, whereas those which make more assumptions have high bias e.g. Logistic or Linear Regression. 

## Variance

The amount to which the prediction of a model would change if a different training dataset was used is called 'Variance'. This means that for each time the model is trained on a dataset, the variability among the predicted values for a given point is the error caused due to variance. If the difference between different runs is small then the variance is low e.g. Logistic or Linear Regression, else the model has high variance e.g. Support Vector Machines (SVM), kNN.
<p align="center">
![Visualizing Bias Vs Variance](/img/bias-variance1.jpg)
*Fig. 1: Visualizing Bias Vs Variance*
</p>

Let's briefly look at this **mathematically**. Let us consider equation Y = f(X)+ ε where Y is the target, X is the feature and ε is the error term. By calculating squared-error loss on a regression fit f'(X) of the model equation, the expected prediction error (Err(x<sub>0</sub>)):

> Err(x<sub>0</sub>) = Irreducible Error (Noise) + Bias<sup>2</sup> + Variance

> Err(x<sub>0</sub>) = σ<sub>ε</sub><sup>2</sup> + [Ef'(x<sub>0</sub>) − f(x0)]<sup>2</sup> + E[f'(x<sub>0</sub>) − Ef'(x<sub>0</sub>)]

## Bias-Variance Tradeoff

Ideally, to obtain a well performing machine learning algorithm, we would want low bias and low variance. However, by observing linear machine algorithms (which have high bias, low variance) and non-linear machine learning algorithms (which have low bias and high variance), we see that we can either have low bias or low variance and not both. Based on the problem we are trying to solve and what is more important to us while solving that problem, we need to optimize and 'trade-off' between the bias and the variance as shown below.
<p align="center">
![Model Complexity](/img/bias-variance2.jpg)
*Fig. 2: Prediction Errors (Bias, Variance) vs Model Complexity*
</p>

## Dealing with Bias and Variance

Managing the bias and variance errors for our algorithms essentially means preventing our model from over-fitting or underfitting. 

Up until the point of 'Optimal Model Complexity' in Figure 2, the bias reduces and variance increases as more parameters are added to the model to learn the given data. Before this point, the model is under-fitting i.e. the model isn't able to capture the underlying trends and hasn't learned from the dataset. 

After that optimal point, the variance starts increasing and bias reduces which means the model is over-learning the particular dataset too well. If another dataset is given to the model, it wouldn't be able to generate good predictions because the learning was specific to the dataset the model had been trained on. 

So the optimal value of complexitity is when the model does not over or under-fit and the value of the total error is minimum. 

There are ways to optimize the selection of model complexitiy and choosing parameters which give the least bias and variance for a given problem: 

* Resampling methods:

    * Cross-validation techniques
        * Hold-out cross-validation
        * K-fold cross-validation
        * Leave-One-Out

    * Bootstrap

Improper splits for the above techniques can lead to high variance. To prevent this, some data Splitting approaches as follows can be used:

* Simple random sampling (SRS)
* Trial-and-error methods
* Systematic sampling
* Convenience sampling
* CADEX
* DUPLEX
* Stratified sampling

    
Further details about these methods and ways these methods can be implemented will be described in the next blog post. Part 2 of this blog post series, will discuss strategies to minimize bias and variance and to make an informed split on datasets before training the models.

#### Further reading:

1. [Data Splitting](https://www.mff.cuni.cz/veda/konference/wds/proc/pdf10/WDS10_105_i1_Reitermanova.pdf)
2. [Understanding the Bias-Variance Tradeoff](http://scott.fortmann-roe.com/docs/BiasVariance.html)