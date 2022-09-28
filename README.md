# *Regression Models in Keras*
## Deep Learning with Neural Networks Using Keras

**In this repository, you can check out the Deep Learning neural networks I built using Keras to model data about concrete compressive strength. Find out more in the follwoing sections!**


__


## Background

In this project, I loaded a dataset about the compressive strength of concrete, split the data into training and testing sets, and built several neural networks...

The project contains four neural networks and reports of their performance compared to a baseline model and a model with normalized data. The four networks are defined and constructed as follows:

### A. Baseline Model
#### *Defining the Network*
- One hidden layer of 10 nodes, and a ReLU activation function
- Use the adam optimizer and the mean squared error as the loss function.

#### *Constructing the Network*
1. Randomly split the data into a training and test sets by holding 30% of the data for testing. You can use the train_test_splithelper function from Scikit-learn.
2. Train the model on the training data using 50 epochs.
3. Evaluate the model on the test data and compute the mean squared error between the predicted concrete strength and the actual concrete strength. You can use the mean_squared_error function from Scikit-learn.
4. Repeat steps 1 - 3, 50 times, i.e., create a list of 50 mean squared errors.
5. Report the mean and the standard deviation of the mean squared errors.


### B. Normalized Baseline Model
#### *Defining and Constructing the Network*
Repeat Part A but use a normalized version of the data by subtracting the mean from the individual predictors and dividing by the standard deviation.

#### *Reporting*
How does the mean of the mean squared errors compare to that from the baseline model without normalized data


### C. Model with Increased Number of Epochs
#### *Defining and Constructing the Network*
Repeat Part B but use 100 epochs this time for training.

#### *Reporting*
How does the mean of the mean squared errors compare to that from the normalized baseline model?


### D. Model with Increased Number of Hidden Layers
#### *Defining and Constructing the Network*
Repeat part B but use a neural network with the following instead:
- Three hidden layers, each of 10 nodes and ReLU activation function.

#### *Reporting*
How does the mean of the mean squared errors compare to that from the normalized baseline model?


---


## Technologies & Usage
This project leverages Python 3.9, Numpy, Scikit-Learn, Pandas, and Keras with the following requirements and dependencies:
- import pandas as pd
- import numpy as np
- from sklearn.model_selection import train_test_split
- import keras
- from keras.models import Sequential
- from keras.layers import Dense
