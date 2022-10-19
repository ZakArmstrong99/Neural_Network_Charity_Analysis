# Neural_Network_Charity_Analysis

## Overview of the analysis:

The purpose of this analysis was to create a deep learning model that uses charity data to predict if potential applicants are sucessful if they are funded by Alphabet Soup. The charity data contains many variables and the data had to be preprocessed before creating the model. After the first model was created, another model was created with the intention of optmizing the data further to give the model more accuracy.

## Results:

### Data Preprocessing
- **What variable(s) are considered the target(s) for your model?**

The target for the model is the IS_SUCESSFUL column which determines if the money was used effectively.

- **What variable(s) are considered to be the features for your model?**

The features are everything in the csv except the target and id variables.

- **What variable(s) are neither targets nor features, and should be removed from the input data?**

The EIN and NAME columns are neither targets nor features and were removed from the data.

### Compiling, Training, and Evaluating the Model
- **How many neurons, layers, and activation functions did you select for your neural network model, and why?**

The model consists of two hidden layers with one containing 80 units and the other containing 30. The two hidden layers used the relu activation function, and the output layer used the sigmoid activation function. These functions were used because they gave better results than the other functions, most likely because the encoded columns ranged from 0 to 1.

- **Were you able to achieve the target model performance?**

I was able the get an accuracy of .725 and a lost of .560.

- **What steps did you take to try and increase model performance?**

In order to increase the model performance, I tried binning the INCOME_AMT column, adding two more hidden layers while changing the units (100, 80, 30, 10) while using tanh and relu, and increased the fit to go for 200 epochs. While my attempts led to some improvement, it was only a minor increase of .729 accuracy.

## Summary: 
