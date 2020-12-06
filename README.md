# Neural_Network_Charity_Analysis

## Overview of the Analysis

We were asked to build a deep learning model that could predict the success of a company in securing funding from Alphabet Soup. This analysis looks at over 34,000 organizations and a multitude of factors in order to predict the investment feasibility of different organizations based on a few criteria.

### Results

#### Data Preprocessing

##### Target Variable

* IS_SUCCESSFUL

##### Feature Variables

* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE
* ORGANIZATION
* INCOME_AMT
* SPECIAL_CONSIDERATIONS
* ASK_AMT


##### Variables Removed

* EIN
* NAME
* STATUS

#### Compiling, Training, and Evaluating the Model

##### Neurons, Layers, and Activation Functions Used

* Neurons - 48, 
* Layers - 3, two hidden and one output layer
* Activation functions - 2, Relu and Sigmoid

##### Target Performance Met?

The target performance was not met, the steps taken to attempt to increase the performance of the model was dropping the Status Column, increasing the number of Bins for the APPLICATION_TYPE and CLASSIFICATION columns, adding a hidden layer, and increasing the number of neurons in the model.

#### Results Summary

Results can be seen below:




##### Next steps
I reccomend attempting a random forest model in order to determine if a similar or higher level of accuracy can be found with less resources.