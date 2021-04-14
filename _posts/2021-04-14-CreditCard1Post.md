---
title: "Credit Card Default Classification Prediction"
date: 2021-04-14
tags: [imbalanced target, data science, binary classification]
header:
  image: "/images/credit card/creditCardImage.jpg"
excerpt: "Data Science, Imbalanced Target, Binary Classification"
mathjax: "true"
---


# Credit Card Default Prediction

## Classification Prediction with Imbalanced Target

**Summary**

The goal of this project was to design predictive binary classification models to predict whether credit card account holders will default on their payments in the next month.  The models address the imbalance in the target variable.  Gradient Boosting and neural network models are highlighted.  The paper and presentation walk through the data understanding and preparation, different models tested, methodology, evaluation and anticipated follow-up steps to the project.  

**Tools**

* Scikit-learn 
* Keras
* Seaborn
* Matplotlib
* Numpy
* Pandas
* Scipy

**Data**

[UCI](http://archive.ics.uci.edu/ml) 

**Models / Methods / Metrics**

* Gradient Boosting Classification 
* Artificial Neural Network
* Random Forest
* Principal Component Analysis
* Log-Transformation and Scaling
* Recall, Log-Loss and Binary Crossentropy Loss

**Results**

The Gradient Boosting Classification model had the best Recall and Log Loss Error scores.  62.43% of the actual default accounts were labeled as true positives.  The Log Loss Error was .4545.  The Artificial Neural Network had a Recall score of .6989 and a binary crossentropy loss of .5958.  These scores resulted from addressing the imbalanced target variable.

## Project Preview

### Exploratory Data Analysis

The EDA shows there are distinctions between the default records and the non-default records.

![image.png](/images/credit card/ECD.png)

![image.png](/images/credit card/Pay1.png)

![image.png](/images/credit card/mean.png)

### Principal Component Analysis

PCA was implemented because of multicollinearity between groups of input variables.

![image.png](/images/credit card/PCA.png)

### Modeling

The imbalanced target variable was addressed by using predicted probabilities for positive outcome based on best classification threshold, and for the Artificial Neural Network, by weighting the the binary target classes.


### Evaluation

**Gradient Boosting Classification, Logistic Regression and Random Forest Models:**

![image.png](/images/credit card/Results1.png)

**Artificial Neural Networks:**

![image.png](/images/credit card/ResultsANN.png)


