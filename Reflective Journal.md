Elda's Entry

This part of the assignment helped me realize that setting up a project the right way is just as important as writing the code.  

While exploring the data, I found out that Colab cell only shows the output from the last line, so I used display() to check the dataset’s shape.  

Splitting the data helped me understand data leakage because the test set should include new patients that the model has not seen before. 



Xinyu's Entry:

This midterm project concerns the machine learning workflow in which data is prepared for model training. By working with the Diabetes Risk dataset for this project, I have gained experience in preparing data for a machine learning model.

One of the insights I gained while working on my part of the project was that different categorical features need to be treated differently. For example, in our dataset of patients, a feature like physical activity level can naturally be converted to a numerical feature while retaining its natural ordering. A feature like the city of a patient’s residence or their gender, however, does not have any natural ordering of categories. One-hot encoding these features would prevent a model from mistakenly treating one category as greater than another.

Another thing that I learned during the project was normalization. When looking at the training data, I noticed that fasting blood sugar and HbA1c level had high positive skewness values of about 0.93 and 0.96, respectively. I used the PowerTransformer to address this issue. After normalization, the two features had skewness values of about -0.02 and -0.01, respectively. The before-and-after plots also helped me understand that one should choose a data preprocessing method based on the data itself and not on prior expectations.

Another method I used was Min-Max scaling on the numerical features to scale them between 0 and 1. I was surprised to find out that there is a difference between normalization and scaling. Normalization can actually change the shape of skewed distributions, whereas Min-Max scaling changes the range of the values but keeps the distribution’s shape mostly intact. This became apparent when I compared the graphs before and after scaling the values.

One of the main things I learned from this assignment is how to avoid data leakage when processing the data. This means that the PowerTransformer and MinMaxScaler were fitted on the training data. Then, the transformations learned from the training data were applied to the test data. The test data should never be used to determine the preprocessing parameters because then the test data would no longer be a representation of the data that the model is expected to encounter when it is run on unseen data.

For the final project, I intend to train and compare different classification models on the same dataset and measure their ability to predict the correct diabetes risk level. Most importantly, I want to see how different preprocessing steps affect the results of the models. The purpose of data preprocessing is to create the best possible input for a model, and there are many ways to reach this goal.

Overall, the project reminded me of an important point about data preparation: it is not just a part of the workflow before training the model. Every step of the preparation influences how the data will be processed by the model. Therefore, it is important to understand the data first and then choose the appropriate method for preparation.
