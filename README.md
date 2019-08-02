# Flight Delays and Cancellations of 2015
SCS 3253 Machine Learning Project

<a href="https://colab.research.google.com/github/Asmaulhushna/2015-Flight-Delays-and-Cancellations/blob/master/Final_project_2015_Flight_Delays_and_Cancellations.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## Team Members
* Asma-Ul-Hushna
* Xubin Zhao
* Yaxal Arenas

## Dataset link
https://www.kaggle.com/usdot/flight-delays

## Project Overview
In 2015 there are lots of flight delays in United States for some reason. Nearly one third of all flights in our data set have delays. The main reasons for flight delays are whether related but in some cases there are also airline or airport related flight delays. In this document we will try to predict if a flight will be Delayed or not on the basis of some given features.

## Notebook Contents
This notebook will explore the data, evaluate some models and draw conclusions. It is divided into the following main sections:

* Setup the environment - seting up the notebook environment.
* Get the data - loading the data set into the notebook.
* Explore the data - exploring the raw flights data.
* Prepare the data - data cleansing, feature selection\reduction\engineering and standardization.
* Model - training and testing various models.
* Evaluate the model - analyzing model results.
* Summary - summarizing the observations and conclusions.

## Models
We used the following classification models to predict arrival delay -

* Logistic Regression
* Random forest
* Decision Tree
* Decision Tree with PCA
* Stochastic Gradient Boosting
* SGDClassifier
* Neural Network

## Comparing Model Accuracy

| Algorithms  | Training Accuracy | Test Accuracy |
| ------------- | ------------- | ------------- |
| Logistic Regression  | 0.94641  | 0.94649 |
| Random Forest   | 0.95903  | 0.94357 |
| Stochastic Gradient Boosting  | 0.94600  |       0.94587|
| SGDClassifier  | 0.94682  |      0.94693 |
| Neural Network   | 0.9450 |          0.94522  |
| Neural Network with PCA   | 0.9442 |     0.94432 |

## Conclusions 
* Stochastic Gradient Boosting is the best Model in terms of accuracy (0.94587), time required(17 min) and memory usage. 
* We can get equivalent performance from SGDClassifier in third of the time taken by Logistic Regression.
* For sufficiently large datasets, it is best to implement SGD Classifier instead of Logistic Classifier to produce similar results in much less time.
* A simple Neural Network has a higher predictive capacity than classic methods (1.14% better).
* Calculation time for a Neural Net with 5 epochs was 2.2 h, too long compared to classic methods.

## Future work 
* Implement regression analysis to predict ARRIVAL_DELAY. 
* Optimize the neural network to decrease time yet not losing accuracy, by changing: number of layers, activation type, number of neurons, batch size, epochs.
