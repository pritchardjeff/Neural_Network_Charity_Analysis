# Neural_Network_Charity_Analysis

## Overview of the Analysis

We were asked to build a deep learning model that could predict the success of a company in using funding from Alphabet Soup. This analysis looks at over 34,000 organizations and a multitude of factors to predict the investment outcomes of different organizations based on a few criteria. The plan would be to use this model in the future to assist with predicting the success of new companies with fund allocation.  

### Results

#### Data Preprocessing

##### Target Variable

* IS_SUCCESSFUL - Was the money used successfully

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
* STATUS - Active vs Inactive did not seem to have a significant impact on the outcome of the analysis

#### Compiling, Training, and Evaluating the Model

##### Neurons, Layers, and Activation Functions Used

* Neurons - 344 neurons were used. The number was determined by the number of samples divided by number of input columns multiplied by an alpha factor for the degrees of freedom. 2 was used for the alpha in this analysis.
* Layers - 3, two hidden and one output layer
* Activation functions - 2, Relu and Sigmoid

##### Target Performance Met?

The target performance was not met, the steps taken to attempt to increase the performance of the model was dropping the Status Column, increasing the number of Bins for the APPLICATION_TYPE and CLASSIFICATION columns, adding a hidden layer, and increasing the number of neurons in the model.

#### Results Summary

Overall, we were able to increase the accuracy of the model from 70.93% to 72.55%.

Pre-Optimized Model:

![Pre_Optimization](https://github.com/pritchardjeff/Neural_Network_Charity_Analysis/blob/main/Pre_Optimization.PNG)

Post-Optimized Model:

![Pre_Optimization](https://github.com/pritchardjeff/Neural_Network_Charity_Analysis/blob/main/Post_Optimization.PNG)

##### Next steps

I recommend attempting a SVM model to determine if a similar or higher level of accuracy can be found with less resources.
