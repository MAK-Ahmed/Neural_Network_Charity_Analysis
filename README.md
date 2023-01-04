# Neural_Network_Charity_Analysis

## Overview
The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations. To do this, we will preprocess the data, compile, train and evaluate the model and finally optimize the model. With this information, the company alphabet soup will be able to identify organization that are worth donating to and those that are high risk.

# Results
* Variables that are considered targets for the model is the IS_SUCCESSFUL column as it contains binary data. 
* There are several variables that are considered features for the model. The columns are listed as follows: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT
* Variables that are neither targets nor features are the EIN, NAME, STATUS and SPECIAL_CONSIDERATIONS and should be removed from the input data
* This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively. I used the activation function ReLU for the hidden layers and sigmoid function for the output layer. 
* The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.
* To increase the performance of the model, I applied bucketing to the feature ASK_AMT and organized the different values by intervals. In addition, increase the number of neurons on in the hidden layers, and different activation functions were tried as well, but the model’s performance had not improved.

## Summary
Unfortunately, the deep learning neural network did not reach the target accuracy of 75%. I would recommend the Random Forest Classifier as a different model to solve fr the classification problem with this method, there are less parameters to optimize that do more require attention, it can combine a multitude of decision trees to generate a classified output against the deep learning model.
