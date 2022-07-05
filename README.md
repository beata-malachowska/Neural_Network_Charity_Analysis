# Neural_Network_Charity_Analysis

##Overview of the analysis: 
The purpose of this analysis was to create an ANN (artificail neural network) model to predict if the company asking for the donation was successful with the project. 

##Results: 

##Data Preprocessing
What variable(s) are considered the target(s) for your model?
IS_SUCCESSFULL
What variable(s) are considered to be the features for your model?

APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested

What variable(s) are neither targets nor features, and should be removed from the input data?
EIN and NAME—Identification columns

##Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Initial model: two hidden layers with 8 and 5 neurons

Optimized model: three hidden layers with 150, 70, and 35 neurons.
I increased the number of neurons and layers to reach desired accuracy - 75%. First hidden layer had around twice as many neurons as input variables, then I tried to reduce them by half. 

Were you able to achieve the target model performance?
No.

What steps did you take to try and increase model performance?
1. Dropped two variables with low variance 'STATUS' and 'SPECIAL_CONSIDERATIONS'.
2. Increased the number of buckets.
3. Increased to three number of hidden layers.
4. Increased the number of neurons for each layer.
5. Increased number of epochs to 500. 
6. Used leaky-relu activation in first hidden layer. 



##Summary: 
My best model achieved accuracy of 0.7446. More data cleaning and using others models like SVM that have better generalization dapability could get better results. 
