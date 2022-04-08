---
title: "Instructor Notes"
---

## Episode 1: A Brief Introduction to Machine Learning

The emphasis here is on brief, and this episode can be done quickly. The lesson deals with some general machine learning concepts using some particular tools that should be of interest to researchers in a range of disciplines. We don't claim to present a comprehensive overview of machine learning. Rather, the goal is to give learners some experience with the techniques they need to apply machine learning to their work. 

The coding here is minimal, but the `kyphosis` data set is introduced to provide a simple example of the framework for supervised learning. Try to use these easy examples to set the tone for live coding and interaction.

Introduce the terms *classification* and *regression*, because these will be used in future episodes. In the field of machine learning, the term "regression" is typically used to describe a situation where the response variable is categorical, which differ from the way statisticians use this term. Episode 2 will illustrate the process of using training and test sets with the *kyphosis* data. 

## Episode 2: Linear and Logistic Regression

It is very likely that learners already are very familiar with linear and logistic regression models, but this episode approaches them from a slightly unorthodox perspective. The goal is to illustrate the framework of supervised learning and introduce the use of training and testing sets. There isn't going to be time to explain the mathematical theory behind these models, nor is it necessary to do so. The focus is on understanding the framework of supervised learning that was introduced in Episode 1.

This is a good time to set the tone for the live coding nature of the workshop; make sure learners are attempting to follow along with you as you type. The challenges should go quickly, but do make sure you wait for learners to come up with the answers themselves. 

In this episode, we form the train and test split using base R. In future episodes, we will use `dplyr::slice`. 


## References

- [CRAN Machine Learning Task View](https://cran.r-project.org/view=MachineLearning)
- [Multiple Logistic Regression](https://rcompanion.org/rcompanion/e_07.html), from the *R Companion*.

{% include links.md %}
