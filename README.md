# Artificial-Neural-Network----predicting-Layality
Creating an Artificial Neural Network with Keras.    
The 'Churn_Modelling.csv' is our dataset file.  
This file contains the data about 10,000 customers of a Bank and thier respective details about them.  
We have to predict whether the person is going to leave the bank based on the respective dependent attributes of a customer.  
We will create an Artificial Neural Network with 2 hidden layers and 6 node each with an output layer having a single node.  

## Data Preprocessing
1. converting categorical data to numbers using LabelEncoder and OneHotEncoder from sklearn.preprocessing  
2. Scaling the data eith standardScaling() also from sklearn.preprocessing

## Creating our Artificial Neural Network
1. Using the Sequential() class from keras.models we created our object of this class.  
2. Add the input layer and first hidden layer using the add method of the Sequential object and the Dense form keras.layers. It contains 6 units  
3. Adding the second hidden layer using the same add function with dense with 6 nodes  
4. adding the last ouput layer with a single node.  
5. We use the compile method of the class to create our ANN.

## Predicting 
use the method predict of the object of class Sequential.  
Convert the output to 0's and 1's  
Calculate accuracy using confusion matrix from sklearn.metrics. 
