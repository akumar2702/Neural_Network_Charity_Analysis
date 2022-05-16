# Neural_Network_Charity_Analysis

## Analysis
### The purpose of this challenge was to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. This model will evaluate all types of input data and produce a clear decision making result. 

## Data Preprocessing:
1. What variable(s) are considered the target(s) for your model?

Checking to see if the target is marked as successful in the DataFrame. The IS_SUCCESSFUL column is considered the target for our model.

2. What variable(s) are considered to be the features for your model?

The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns are considered to be the features of our model.

3. What variable(s) are neither targets nor features, and should be removed from the input data?

The EIN, NAME, STATUS, and SPECIAL_CONSIDERATION columns are neither targets nor features and should be removed from the input data.

## Compiling, Training, and Evaluating the Model:
4. How many neurons, layers, and activation functions did you select for your neural network model, and why?

I selected 120 neurons with a sigmoid function for my first layer, 100 nuerons with a ReLU function for the second, then 80 neurons with a tanh classification for the third and 60 for the fourth, and a sigmoid function for the outer layer. I chose to change the activation function for the first layer because it increased the model's performance.

<img width="1074" alt="Screen Shot 2022-05-16 at 6 39 56 PM" src="https://user-images.githubusercontent.com/95302013/168694260-2846adb6-1dca-4a3d-bb76-2ead035b99b6.png">


5. Were you able to achieve the target model performance?

The target was 75% and I only achieved an accuracy of 74%.

<img width="1116" alt="Screen Shot 2022-05-16 at 6 42 17 PM" src="https://user-images.githubusercontent.com/95302013/168694199-9259b518-2ac9-43a0-8862-9d7ac1c7cbdc.png">


6. What steps did you take to try and increase model performance?

We tried to increase the model performance by dropping more columns, creating more bins for rare occurances in columns, decreasing the number of values in some bins, adding more neurons to the hidden layers, using a differnet activation function, and increasing the number of epochs. We tried more hidden layers and increased epochs to 100 to increase model performance. Other activations were tried such as tanh.Linear activation produced the worst accuracy, around 28%. The relu activation at the early layers , tanh activation in the middle and sigmoid activation at the latter layers gave the best results.

## Summary:

A random forest model could solve this classification problem by randomly sampling the preprocessed data and building several smaller, simpler decision trees. The relu, tanh and sigmoid activations yielded a 74.11% accuracy.
