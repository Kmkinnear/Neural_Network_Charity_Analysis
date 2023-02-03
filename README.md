# Neural_Network_Charity_Analysis

## Overview

The purpose of this assignment was to take our charity dataset and see if we could create an effective neural network that is capable of predicting whether applicants will be successfull if they are funded by Alphabet Soup. We build an initial neural network and then attempt to optimize it by testing three additional neural network models. We'll do that by adding more neurons to our hidden layers, using different activation functions in our models, and we also used an approach of adding another hidden layer. We also tried adjusting the number of epochs that would run in each model.

## Results:

### Data Preprocessing

<img width="415" alt="image" src="https://user-images.githubusercontent.com/110848660/216507261-39dc5346-cf65-408a-8947-9a9e14ba2f81.png">

- What variable(s) are considered the target(s) for your model? We can see in the picture above that the target variable in this "IS_SUCCESSFUL" column.

- What variable(s) are considered to be the features for your model? The feature variables would be the remaining variables in our database. These were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

<img width="728" alt="image" src="https://user-images.githubusercontent.com/110848660/216507921-f965db27-3794-4c7b-9976-da173234bf27.png">

- What variable(s) are neither targets nor features, and should be removed from the input data? We had two variables in this challenge that were neither a target or a feature. Those two variables were EIN and NAME. We ended up dropping those two variables from our data set as you can see in the picture below.

<img width="432" alt="image" src="https://user-images.githubusercontent.com/110848660/216507744-22e0a095-9b98-43f1-86e4-33a977e0382d.png">


### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?

Original Model

<img width="640" alt="image" src="https://user-images.githubusercontent.com/110848660/216508136-9c52ba2d-2a07-4b2f-b253-716ea7912f29.png">

- Neurons: 1st Hidden Layer - 10, 2nd Hidden Layer - 5
- Layers: 4. Input Layer, Hidden Layer #1, Hidden layer #2, Output Layer
- Activation functions: Relu(Hidden Layer #1), Relu(Hidden Layer #2), Sigmoid(Output Layer)

Optimization Model 1

<img width="638" alt="image" src="https://user-images.githubusercontent.com/110848660/216508185-77fd8c4d-769f-47de-bcef-0290ff6dab6e.png">

- Neurons: 1st Hidden Layer - 15, 2nd Hidden Layer - 10
- Layers: 4. Input Layer, Hidden Layer #1, Hidden layer #2, Output Layer
- Activation functions: Tanh(Hidden Layer #1), Relu(Hidden Layer #2), Sigmoid(Output Layer)

Optimization Model 2

<img width="656" alt="image" src="https://user-images.githubusercontent.com/110848660/216508328-172811c3-0357-491d-ba1d-f7913c357330.png">

- Neurons: 1st Hidden Layer - 15, 2nd Hidden Layer - 10, 3rd Hidden Layer - 8
- Layers: 5. Input Layer, Hidden Layer #1, Hidden layer #2, Hidden Layer #3, Output Layer
- Activation functions: Tanh(Hidden Layer #1), Relu(Hidden Layer #2), Relu(Hidden Layer #3), Sigmoid(Output Layer)

Optimization Model 3

<img width="625" alt="image" src="https://user-images.githubusercontent.com/110848660/216508261-fc1c0f3c-f00f-45bc-abce-95263e4ad7d4.png">

- Neurons: 1st Hidden Layer - 20, 2nd Hidden Layer - 8, 3rd Hidden Layer - 12
- Layers: 5. Input Layer, Hidden Layer #1, Hidden layer #2, Hidden Layer #3, Output Layer
- Activation functions: Tanh(Hidden Layer #1), Relu(Hidden Layer #2), Sigmoid(Hidden Layer #3), Sigmoid(Output Layer)
 
Were you able to achieve the target model performance? - We were unable to achieve the target model performance metric of 75% in either of our 4 neural networks that we created. 

The results were as follows:
   - Original Model: 72.7%
   - Optimization Model 1: 73.1%
   - Optimization Model 2: 73.4%
   - Optimization Model 3: 72.8%
    
- What steps did you take to try and increase model performance? - We tried a few different steps to try and increase our model's performance. We tried adding more neurons to our hidden layers. We also experimented with different activation functions in our models across different layers. We also tried adding additional hidden layers. Lastly we tried adjusting the number of epochs that would run in each model to see if we could get any improved results. We saw different numbers in each model although we still fell short of the goal of 75% accuracy.

### Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

We tried 3 additional neural network models from our original model. We did not see any significant change despite adding additional layers, adding neurons, changing activation functions, and adjusting the number of ephocs. This makes me believe that we should take a different approach in future analysis and try some different approaches to get out accuracy score up. We could further adjust our input data by dropping columns that don't have a strong influence on the outcome and may be skewing the data. There's also a chance that there are some outliers in the data that could be throwing our model off. One other approach we could use is to adjust the number of bins that we put our binned data in. We can also adjust the size of those bins to create a different number of unique values.
