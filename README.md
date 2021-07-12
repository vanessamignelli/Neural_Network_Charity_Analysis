# Neural_Network_Charity_Analysis

## Overview
The purpose of this project was to create a binary classifier capable of predicting sucessful applicants to receive funcding from a company. This was completed by leveraging the company's metadata of over 34,000 organizations that have received funding. With this information, the data was pre-processed, trained and then used to make predictions using a neural network. The performance of the model was then evaluated.

## Results: 

### Data Preprocessing
What variable(s) are considered the target(s) for your model?
- The target for this model was a column called 'IS_SUCCESSFUL' which is binary classified show if the money was used effectively

What variable(s) are considered to be the features for your model?
- APPLICATION_TYPE: application type
- AFFILIATION: affiliated sector of industry
- CLASSIFICATION: government organization classification
- USE_CASE: use case for funding
- ORGANIZATION: organization type
- STATUS: active status
- INCOME_AMT: income classification
- SPECIAL_CONSIDERATIONS: special consideration for application
- ASK_AMT: funding amount requested

What variable(s) are neither targets nor features, and should be removed from the input data?
- the 'EIN' and 'NAME' columns which are identification columns are neither target nor features, so they were removed

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- neurons: 80 in first layer, 30 in second layer
- layers: 2 hidden layers, 1 output layer
- activation function: 'relu' in hidden layers, 'sigmoid' in output layer

Were you able to achieve the target model performance?
- The target performance was an accuracy of above 75%, with this model 72.2% accuracy was achieved - therefore the target was not reached

What steps did you take to try and increase model performance?
- remove additional variables from the target variables to try and reduce noise (removed: active status, special considerations and income amount)
- added additional neurons to hidden layers (30 additional neurons added to the second hidden layer)
- added an additional hidden layer
- changed the hidden layer activation function to 'tanh'

## Summary
Overall, the highest accuracy the learning model was able to acheive was 72.5%, which would indicate that the model would be able to accurately predict whether an ivestment would be successful or not 72.5% of the time. Because the accuracy isn't as high as we would like it to be, another model that could be used is Random Forests. Random Forests are similar to neural networks but have the ability to easily handle outliers so may prove more effective in predicting accurately in this instance. 
