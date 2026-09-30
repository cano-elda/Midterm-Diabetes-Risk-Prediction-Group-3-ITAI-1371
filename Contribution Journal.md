Elda's Entry  



For this assignment, I created our team’s Github repository and uploaded the original diabetes risk CVS file to a data folder so everyone could access it using the same link.  

I also created a one-page document with the original dataset URL and explaining the dataset and our project goals. Next, I created a Google Colab notebook, imported the libraries – pandas, NumPY,  

Matplotlib, scikit-learn, imbalanced-learn – and loaded the CVS with pandas. I review the dataset’s shape, column types, and missing values with df.info(). After this, I split the data into  

70% training and 30% testing. I created a histogram chart that shows how the data is spread out before pre-processing. Finally, I processed the missing values by using the mode for the smoking  

status and income bracket and adding an “Unknown” category for alcohol consumption. These replacement values should be calculated only from the training set to prevent data leakage.

