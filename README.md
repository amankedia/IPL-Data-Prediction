# IPL-Data-Prediction

This repository contains code for my exploration with a modified IPL dataset.

## Data
The data pertains to matches between teams and provides information such as Wind Speed, Humidity, Number of 4s and 6s hit in each innings of the match.

It is a mix of Categorical and Numeric/Continuous data.

The prediction column states which team won the match.

The train and test files are provided separately which add to the challenges explained below.

## Problem Statement

Building a model which could predict the Winner of the match provided the necessary data.

## Preprocessing Applied

1. Normalizing Continuous data using StandardScalar
2. One Hot Encoding of Categorical data using Get dummies method from Pandas.

## Challenges

The test file for certain categorical attributes contains data which is not present in the train file.

Hence, a basic One Hot Encoding on the train data followed by application on both train and test data would not suffice.

### Possible Solutions

1. Use a <UNK> one hot column for categorical values not present in the training data but present in test/inference data.

2. Combine train and test data to have a holistic view of the categorical attributes.

In this study/experimentation, we have combined the train and test data to identify unique values.

## Classification

### Algorithms tried

1. k-Nearest Neighbors

2. Decision Trees

3. Random Forests

4. Support Vector Machines with Linear and RBF kernels

## Results

An F1-Score of 90.789 % could be achieved on the test data.


For any feedback/queries reach out to me on amankedia.sap@gmail.com
