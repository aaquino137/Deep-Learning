# Deep-Learning
Neural Networks(NN)

The purpose of using this type of model on the datset is to make predictions that we otherwise wouldn't be able to make as efficiently using regular methods.

Format images are included in thee report to display NN correction. 

Below is an image of how the data was restructered to include the 'NAME' column that had initially been dropped
![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/129812a1-058c-47ce-9a79-95930f93625c)
![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/24a42c7c-fda6-4e36-a167-7c9b7bb0a0ab)

Afterwards, the Neural Network was changed for optimization purposes
![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/52b265c0-58e0-40c9-841c-4fdcb9281cf8)
![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/73c899a3-4ea2-4cc2-a023-645a3e3fa407)

Below is an example of an attempt that was unable to produce a NN with an accuracy score of 75%.
![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/7f35ff14-382a-48dd-bc5d-580b69eab724)


![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/99f44ac7-9a0f-4ec2-810f-7b7bb46b135f)



![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/e317860e-2fd6-49eb-ae5e-dcd28866d6e3)

![image](https://github.com/aaquino137/Deep-Learning/assets/120290921/2d1c50cc-0b47-400a-b615-8fff4409ea47)



Data Preprocessing

- What variable(s) are the target(s) for your model?
The target(s) for your model include the column 'IS_SUCCESSFUL'.

- What variable(s) are the features for your model?
Features of the model include 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT','SPECIAL_CONSIDERATIONS', 'ASK_AMT', 'IS_SUCCESSFUL'.

- What variable(s) should be removed from the input data because they are neither targets nor features?

Since 'EIN' and 'NAME' are non-beneficial ID columns they were removed as they are neither targets nor features



Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
For the original neural network model 2 layers with 80 and 30 neurons were used. As the activation function Relu was used.

- Were you able to achieve the target model performance? 
Target model performance was not achieved therefore efforts were made to optimize the model.
- What steps did you take in your attempts to increase model performance?
To increase model performance tanh the number of neurons were changed, tanh was used as an activation function and additional hidden layer was added. Also, Data was restructured to value count NAME as opposed to APPLICATION_TYPE, which revealead that NAME is a more relevant feature.

 
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall the deep learning model served its function of predict whether applicants will be successful if funded by Alphabet Soup. Unfortunately, despite optimizing the model the Accuracy only improved slightly past 75% Accuracy. Since this is a binary classification problem  a support vector machine can be used to sepearte whether the applicants were successful or not.



