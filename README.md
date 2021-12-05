# Neural_Network_Charity_Analysis

This project was done using Google Colab vs. Jupyter Notebook due to the technical incompatability between Tensorflow and Mac's M1 processor chip. 

**Overview of the loan prediction risk analysis**

Looking at a dataset from a fictional non-profit, Alphabet Soup, we are analyzing over 34,000 organizations who have recieved funding from the non-profit. Our objects were as follows:

Deliverable 1: Preprocessing Data for a Neural Network Model
Deliverable 2: Compile, Train, and Evaluate the Model
Deliverable 3: Optimize the Model

**Results**

_Data Preprocessing_

What variable(s) are considered the target(s) for your model? In this model, I am considering the IS_SUCCESSFUL column as a target.  

What variable(s) are considered to be the features for your model? In this model, I am considering the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns to be features.

What variable(s) are neither targets nor features, and should be removed from the input data? In this model, the EIN, NAME, STATUS, and SPECIAL_CONSIDERATION columns are neither targets nor features. 

_Compiling, Training, and Evaluating the Model_

How many neurons, layers, and activation functions did you select for your neural network model, and why?
For the first layer, we chose 100 neurons with a sigmoid function. For the second layer, 40 nuerons we chosen with a ReLU function. For the third and final layer, 15 neurons were chosen also with a ReLU function. For the first layer, we went with the sigmoid function due to its historical model performance. 

![Challenge 19_Neural_Layers 1](https://user-images.githubusercontent.com/86584404/144731911-c4afb389-918a-4dbe-8b99-16e8593f0c2d.jpeg)

Were you able to achieve the target model performance?

The target model accuracy goal was 75%. However, mine came in at 53%.

![Challenge 19_Del_3 1](https://user-images.githubusercontent.com/86584404/144731920-2eb69af0-0a64-45d5-8506-19787343fa95.jpeg)

What steps did you take to try and increase model performance?

I worked to increase the layers of the models (doubled each layer, respectively). In increasing the model's layers the accuracy came in even lower at 47%. 
![Challenge 19_Del_3_Accuracy 2](https://user-images.githubusercontent.com/86584404/144732153-9d0184c1-b859-4aed-a0c4-dacc9e723694.jpeg)

As well, I increased the number of epochs to 200 and the save frequency of the model from 4,000 to 5,000. This step moved our accuracy from 47% back to 53%. 
![Challenge 19_Del_3_Optimization 2](https://user-images.githubusercontent.com/86584404/144732246-8e743d45-586e-4788-8f60-62c5bc94e2aa.jpeg)


**Summary**

In manipulating the neurons, epochs and potential noisy features, you can increase or decrease your model's performance. As well, one may desire to implement a random forest classification model to sample random data for additional unbiased accuracy.
