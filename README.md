# Neural_Network_Charity_Analysis

## Overview of the Project: 

From Alphabet Soup’s business team, We have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. .The project will use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

### Deliverables

The project consists of four deliverables

a. Deliverable 1: Preprocessing Data for a Neural Network Model

b. Deliverable 2: Compile, Train, and Evaluate the Model

c. Deliverable 3: Optimize the Model

d. Deliverable 4: A Written Report on the Neural Network Model (README.md)

### Data Preprocessing

a. What variable(s) that are considered the target(s) for your model?

The variable we are targeting in this module is the IS_SUCCESSFUL column.

b. What variable(s) are considered to be the features for your model

The features that we are using are every column except that includes
  * AFFILIATION
  * APPLICATION_TYPE
  * ASK_AMT
  * CLASSIFICATION
  * INCOME_AMT
  * ORGANIZATION
  * SPECIAL_CONSIDERATIONS
  * STATUS
  * USE_CASE

c. What variable(s) are neither targets nor features,and should be removed from the input data?

First features we drop are the 'EIN' & 'NAME' because we expect both features to have little to do with our outcome.

### Compiling, Training, and Evaluating the Model

a. How many neurons, layers, and activation functions did you select for your neural network model, and why?

This model is made with an input features & two hidden layers. The first hidden layer has 80 neurons, the second has 30 there is also an output layer. Each layer has an activation function. The first and second hidden layers have an activation function "relu" & the output layer is "sigmoid".
![Del2_Test.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Del2_Test.png)

b. Were you able to achieve the target model performance?

Although we the target for the model was to be 75% or above, however the accuracy only 72.60%
![Test_1.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Test_1.png)

c. What steps did you take to try and increase model performance?

Further testing was done with by adding hidden layers, changing the activation type, changing the number of epochs and changing the number of neurons in each layer.

* Optimised Model 1: 72.58%
![Optimisation_1.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_1.png)

![Optimisation_Test1.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_Test1.png)

* Optimised Model 2: 72.58%
![Optimisation_2.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_2.png)
![Optimisation_Test2.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_Test2.png)

* Optimised Model 3: 72.6%
![Optimisation_3.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_3.png)
![Optimisation_Test3.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_Test3.png)

Likewise a dynamic tuned models that statically and dynamically selected inputs, layers, neurons, and activations and yeilded following results.

* Optimised Model 4: 73.50%
![Optimisation_4.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_4.png)
![Optimisation_Test4.png](https://github.com/Shikharbhd/Neural_Network_Charity_Analysis/blob/main/Resources/Images/Optimisation_Test4.png)

## Summary:

Although we the target for the model was to be 75% or above,  the accuracy was only 72.60%. Subsequent optimisation resulted in the following outcomes
* Optimised Model 1: 72.58%
* Optimised Model 2: 72.58%
* Optimised Model 3: 72.6%
* Optimised Model 4: 73.50%

### recommendation: 

To further investigate these tests we recommend alternative, non-sequential hyperparameter models. Another means of improving accuracy is to have more datapoints. Although we did not boost success rate to 75%, we have minimized loss using these tuned models.
