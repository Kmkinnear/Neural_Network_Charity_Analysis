# Neural_Network_Charity_Analysis

## Overview

The purpose of this assignment was to take our charity dataset and see if we could create an effective neural network that is capable of predicting whether applicants will be successfull if they are funded by Alphabet Soup. We build an initial neural network and then attempt to optimize it by testing three additional neural network models. We'll do that by adding more neurons to our hidden layers, using different activation functions in our models, and we also used an approach of adding another hidden layer. We also tried adjusting the number of epochs that would run in each model.

## Results:

### Data Preprocessing

<img width="415" alt="image" src="https://user-images.githubusercontent.com/110848660/216507261-39dc5346-cf65-408a-8947-9a9e14ba2f81.png">

- What variable(s) are considered the target(s) for your model? We can see in the picture above that the target variable in this "IS_SUCCESSFUL" column.

- What variable(s) are considered to be the features for your model? The feature variables would be the remaining variables in our database. These were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

- What variable(s) are neither targets nor features, and should be removed from the input data? We had two variables in this challenge that were neither a target or a feature. Those two variables were EIN and NAME. We ended up dropping those two variables from our data set as you can see in the picture below.

<img width="432" alt="image" src="https://user-images.githubusercontent.com/110848660/216507744-22e0a095-9b98-43f1-86e4-33a977e0382d.png">


### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Were you able to achieve the target model performance?
- What steps did you take to try and increase model performance?

### Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
