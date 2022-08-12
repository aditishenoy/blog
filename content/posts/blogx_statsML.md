---
title: "Statistical Learning"
date: 2021-05-24T21:46:42+02:00
draft: true
---

Input variables, predictors, independent variable, features
Output variable, dependent variable or response

Quantitative output variable Y and p input variables $X1, X2,...Xp$ and there is some relationship between Y and $X1, X2,...Xp$ such that 

$$Y = f(X) + b$$
where $f$ gives systematic information about $X$ and $b$ is the error term. 

Essentially, statistical learning includes ways to estimate $f$ and thereby estimate the how $X$ is related to $Y$. 

There are two reasons to estimate $f$:

1) Prediction 

The estimated value 
$$E(Y^*-Y)^2 = E[f^*(X)+b - f(X)]^2$$
$$E(Y^*-Y)^2 = [f^*(X)- f(X)]^2 - Var(b)$$
where $Y=f(X)$

$[f^*(X)- f(X)]^2$ - reducible error
$Var(b)$ - irreducible error

Focus is to minimize reducible error because irreducible error may contain unmeasured terms which affect the value of $Y$

2) Inference - To understand the relationship between Y and $X1, X2,...Xp$ i.e. how does Y change as a function of $X$

Depending on if goal is prediction, inference or both, different models for estimating f can be used. 

Fig to show Linear models are interpretable, less accurate, Non-linear (complex) models are more accurate but less interpretable


Estimating f (Parametric vs Non-parametric approaches)

1) Parametric approach has two steps (a) making an assumption about the form of $f$ (is it a linear model in the form $f(X)=\beta0+\beta1X1 +\beta2X2+...+\beta nXn$) (b) fit the model (i.e. find values for $\beta, \beta1,...,\beta n$) by (eg. least squares). So a parametric approach is where estimation of $f$ means estimating the values of parameters in a linear model. A downside of parametric approach is that there is a possibility that the estimated value is far from the true value. If we choose a more flexible model which can fit more forms of $f$, the number of parameters start increasing and can lead to overfitting. 
2) Non-parametric approaches involves not making assumptions about the form of $f$ and therefore have the advantage of fitting multiple forms of $f$ but a very large number of data points needed to estimate $f$. 