# Neural_Network_Charity_Analysis
Tools: Python, Scikit-Learn, TensorFlow, Keras, Jupyter Notebook

# Charity Analysis through Neural Network and Deep Learning Models
## Overview
The purpose of this analysis is to build a Deep Learning Neural Network that can correctly predict if a charity is worth providing a loan with at least 75% accuracy - using the TensorFlow platform in Python.

In order to perform this task we must:
* Preprocess the data for a Neural Network Model
* Compile, Train, and Evaluate the model
* Optimize the model through micro adjustments

## Results
Data Preprocessing
* The target variable in the dataset was the "IS_SUCCESSFUL" column
* The features in the dataset were every column other than the "IS_SUCCESSFUL" column, which was dropped.
* The variables in the dataset were the "EIN" and "NAME" columns. These did not provide any useful input into the model and were dropped
* Comiling, Training, and Evaluating the Model

The first Deep Learning Neural Network model I used had 2 hidden layers, containing 80 and 30 neurons. I used this number as suggested by the instructions for the first attempt.
* The output layer contained 1 neuron
* I used Relu activation functions for the hidden layers and Sigmoid activation for the output layer
* The original attempt achieved 72.6% accuracy with about 55% loss.
* In my first optimization attempt I used 3 hidden layers with 80, 50, and 20 neurons respectively, achieving 72.6% accuracy and 56% loss
* In my second optimization attempt I used 3 hidden layers with 150, 100, and 50 neurons respectively, achieving 72.5% accuracy and 57% loss
* In my third optimization attempt I used 3 hidden layers again, with 200, 150, and 100 neurons, achieving 72.5% accuracy and 57% loss

## Summary
Based on the optimization attempts, which decreased in overall accuracy and increase in loss, I can conclude that adding layers and neurons do not increase the effectiveness of the model with this dataset. In order to increase model performance above 75% I would recommend removing additional "noisy" features to result in optimization.
