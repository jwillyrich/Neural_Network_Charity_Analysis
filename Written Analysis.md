# Neural Network Charity Analysis
Module 20 Challenge - Supervised Machine Learning

## Overview
Alphabet Soup, a fictious non-profit fund-raising company is trying to determine which candidates will be successful if funded. Using neural networks and a variety of techniques I will attempt to create a Machine Learning module to find the best fit. The dataset provided contains 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

The overview is to take the data found inside the csv charity file and ingest the data into a Pandas dataframe. From there a few columns are removed ['EIN', 'NAME'] because they do not add into the overall feature data. The specific columns to target for the machine learning module are ['IS_SUCCESSFUL']. 

## Compiling, Training, and Evaluating the Model: 
In an attempt to improve the models accuracy, I made several changes to the data models. Below is a breakdown of the different activation models and different layers changed in layers to improve the results.</br>
1st attempt: </br>
hidden_nodes_layer1 = 80 </br>
hidden_nodes_layer2 = 40 </br>
hidden_nodes_layer3 = 40 </br>
Hidden Layer activation was set to "relu" </br>
Output layer activation was set to "sigmoid" </br> 
epochs=150 </br>
Accuracy: 0.7253644466400146 </br>

2nd attempt: </br>
hidden_nodes_layer1 = 80 </br>
hidden_nodes_layer2 = 40 </br>
hidden_nodes_layer3 = 40 </br>
Hidden Layer activation was set to "selu" </br>
Output layer activation was set to "sigmoid" </br>
epochs=200 </br>
Accuracy: 0.724781334400177 </br>

3rd attempt: </br>
hidden_nodes_layer1 = 60 </br>
hidden_nodes_layer2 = 30 </br>
hidden_nodes_layer3 = 20 </br>
epochs=200 </br>
Hidden Layer activation was set to "tanh" </br>
Output layer activation was set to "sigmoid" </br>
Accuracy: 0.7246647477149963 </br>
</br>

# Summary
The overall model did not improve in any meaningful way. Additional computations need to be made to improve the accuracy to 83% or above.
