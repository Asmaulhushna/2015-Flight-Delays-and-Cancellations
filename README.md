# 2015-Flight-Delays-and-Cancellations
Machine Learning Project - Comparing models to predict Flight Delays

## Team Members
Asma-Ul-Hushna
Xubin Zhao
Yaxal Arenas

## Project Overview
In 2015 there are lots of flight delays in United States for some reason. Nearly one third of all flights in our data set have delays. The main reasons for flight delays are whether related but in some cases there are also airline or airport related flight delays. In this document we will try to predict if a flight will be Delayed or not on the basis of some given features.

## Notebook Contents
This notebook will explore the data, evaluate some models and draw conclusions. It is divided into the following main sections:

Setup the environment - seting up the notebook environment.
Get the data - loading the data set into the notebook.
Explore the data - exploring the raw flights data.
Prepare the data - data cleansing, feature selection\reduction\engineering and standardization.
Model - training and testing various models.
Evaluate the model - analyzing model results.
Summary - summarizing the observations and conclusions.

## Models
We will apply the following classification models to our dataset

Logistic Regression
Random forest
Decision Tree
Decision Tree with PCA
Stochastic Gradient Boosting
SGDClassifier
Neural Network

## Conclusions 
The percentage of planes late in 2015 is 35.86 The percentage of planes right on time in 2015 is 2.17 The percentage of planes that arrived ahead of time in 2015 is 60.16.
Stochastic Gradient Boosting is the best Model in terms of accuracy (0.94587), time required(21 min) and memory usage. 
We can get equivalent performance from SGDClassifier in third of the time taken by Logistic Regression.
For sufficiently large datasets, it is best to implement SGD Classifier instead of Logistic Classifier to produce similar results in much less time.
A simple Neural Network has a higher predictive capacity than classic methods (1.14% better).
Calculation time for a Neural Net with 5 epochs was 2.2 h, too long compared to classic methods.

## Future work 
Implement regression analysis to predict ARRIVAL_DELAY. 
Optimize the neural network to decrease time yet not losing accuracy, by changing: number of layers, activation type, number of neurons, batch size, epochs.