---
title: "Instructor Notes"
---

## Episode 1: A Brief Introduction to Machine Learning

The emphasis here is on "brief." This episode can be done quickly. The lesson deals with some general machine learning concepts using some particular tools that should be of interest to researchers in a range of disciplines. We don't claim to present a comprehensive overview of machine learning. Rather, the goal is to give learners some experience with the techniques they need to apply machine learning to their work. 

The coding here is minimal, but the `kyphosis` data set is introduced to provide a simple example of the framework for supervised learning. Try to use these easy examples to set the tone for live coding and interaction.

Introduce the terms *classification* and *regression*, because these will be used in future episodes. In the field of machine learning, the term "regression" is typically used to describe a situation where the response variable is categorical, which differ from the way statisticians use this term. Episode 2 will illustrate the process of using training and test sets with the *kyphosis* data. 

## Episode 2: Linear and Logistic Regression

It is very likely that learners already are very familiar with linear and logistic regression models, but this episode approaches them from a slightly unorthodox perspective. The goal is to illustrate the framework of supervised learning and introduce the use of training and testing sets. There isn't going to be time to explain the mathematical theory behind these models, nor is it necessary to do so. The focus is on understanding the framework of supervised learning that was introduced in Episode 1.

This is a good time to set the tone for the live coding nature of the workshop; make sure learners are attempting to follow along with you as you type. The challenges should go quickly, but do make sure you wait for learners to come up with the answers themselves. 

In this episode, we form the train and test split using base R. In future episodes, we will use `dplyr::slice`. 

The formula syntax for `lm` and `glm` will also be used in future episodes for other types of models.

## Episode 3: Decision Trees

This episode introduces decision trees, which will be the basis for the more complex models that we will consider in later episodes (random forests and gradient boosted trees). 

Consider having learners work on challenges in groups, especially for the third challenge (Predicted Probabilities).

## Episode 4: Random Forests

Instructions for downloading the wine data are on the [setup](../setup.html) page. The methods we will consider are often used on data sets with more rows and columns, but we are using this relatively small data set to avoid memory and time constraints.

Of the last three challenges, the most important for future episodes is the White Wine challenge, because we plan to compare the RMSE of random forests with gradient boosted trees, before and after tuning.

## Episode 5: Gradient Boosted Trees

There won't be time to get in to the particulars of what exactly the XGBoost algorithm is doing at each stage. The [references](#references) below are a good place to direct interested learners. Suffice it to say that the algorithm works in stages, or *iterations*, and attempts to improve the model at each iteration. 

Make sure to leave time for the White Wine challenge, because we want to compare its RMSE with the random forest challenge in Episode 4 and the tuned model in Episode 6.

## Episode 6: Cross Validation and Tuning

This episode presents a somewhat systematic way to tune parameters in an XGBoost model, but it is not a comprehensive guide to the subject. In order to be prepared for questions, instructors should be familiar with the last four references in [the list](#references) at the end of the instructors guide.

Some of the examples in this episode will take several minutes to run, depending on the speed of your computer. Instructors may wish to pare down the grid search candidates to save time. Have a plan for something to do while you wait for these examples to finish.

Learners may not recall/know how to write functions in R, so be prepared to help them with the second challenge. Mention that the function could also be written to allow other settings to be passed as additional arguments, if desired.

Advise learners to start with small grids when doing the final challenge, so that they don't end up having to wait for their `GridSearch` functions to finish.


## References

- [CRAN Machine Learning Task View](https://cran.r-project.org/view=MachineLearning)
- [Multiple Logistic Regression](https://rcompanion.org/rcompanion/e_07.html), from the *R Companion*.
[Manual on Setting Up, Using, and Understanding Random Forests](https://www.stat.berkeley.edu/~breiman/Using_random_forests_V3.1.pdf), Leo Breiman.
-  [XGBoost Presentation vignette](https://cran.r-project.org/web/packages/xgboost/vignettes/xgboostPresentation.html) 
- [Introduction to Boosted Trees](https://xgboost.readthedocs.io/en/stable/tutorials/model.html), XGBoost documentation.
- [Notes on XGBooost Parameter Tuning](https://xgboost.readthedocs.io/en/stable/tutorials/param_tuning.html)
- [Documentation for XGBoost Parameters](https://xgboost.readthedocs.io/en/stable/parameter.html)
{% include links.md %}
- [An Introduction to Statistical Learning](https://hastie.su.domains/ISLR2/ISLRv2_website.pdf), by James, Witten, Hastie, and Tibshirani.
- [Laurae++: notes on XGBoost/LightGBM parameters](https://sites.google.com/view/lauraepp/parameters)


