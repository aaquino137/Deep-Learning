# Deep-Learning
Neural Networks

Format images in the report so that they display correction (2)


Explain the purpose of the analysis (4)

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



