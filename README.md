# Neural_Network_Charity_Analysis

## overview

The purpose of this analysis is to use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

###Data Preprocessing

What variable(s) are considered the target(s) for your model?

- The target variable for the model was the "IS_SUCCESSFUL" category.

What variable(s) are considered to be the features for your model?

- The original model considered the following columns as features: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, IS_SUCCESSFUL.

What variable(s) are neither targets nor features, and should be removed from the input data?

-For this model we removed the EIN and NAME columns.

###Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

-There are two hidden node layers with 80 input//neurons in the first layer with the second smaller layer containing 30 input/neurons. The neural network model contains 2 hidden layers and an output layer each with activation functions: "relu" / "relu" and "sigmoid".

Were you able to achieve the target model performance?

- The original models performance fell short of the 75% target. The accuracy recorded was 72.5% with a loss of 55.9%.

What steps did you take to try and increase model performance?

- Attempt #1: An additional variable was removed from the data set, "SPECIAL_CONSIDERATIONS"
- Attempt #2: Adjusted the amount of neurons and layers. The neurons on the first layer were adjusted to 100, the second layer 50 and an added third layer with 25. The third hidden layer was added with an activation of "relu"
- Attempt #3: The output layer was changed from "sigmoid" to "tanh".

## Summary

The deep learning model failed to reach its target accuracy at 75%. The attempts to optimize the model also failed to reach the target of 75%. THe combined attempts to optimize only slightly improved upon the accuracy of the original model, increasing from 72.5% to 72.8%.

The variables we're working with could be researched further. For example the ASK_AMT has 8,747 unique values. It could be possible to dig deeper into these amounts and create bins for ranges. This would decrease the amount of unique values and may improve the overall accuracy of the model as well.
