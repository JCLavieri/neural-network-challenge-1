
# Student Loan Risk with Deep Learning

This exercise demonstrates how to use deep learning to predict the risk of student loan default. The dataset used in this exercise is the LendingClub dataset, which contains information on over 100,000 student loans.

## Data Preprocessing

The data preprocessing steps involved in this exercise are as follows:

1. **Missing Values**: Missing values in the dataset are imputed using the following strategies:
    * For numerical columns, the missing values are imputed using the median value of the column.
    * For categorical columns, the missing values are imputed using the most frequent value of the column.
2. **Feature Engineering**: The following feature engineering steps are performed:
    * The `earliest_cr_line_date` column is converted into a numerical feature by calculating the difference between the loan origination date and the earliest credit line date.
    * The `issue_d` column is dropped as it is not relevant for predicting loan risk.
3. **Categorical Encoding**: Categorical features are encoded using one-hot encoding.
4. **Train-Test Split**: The dataset is split into training and testing sets using a 70/30 split.

## Model Training

A deep learning model is trained on the training set to predict the risk of student loan default. The model architecture used is a simple neural network with two hidden layers.

## Model Evaluation

The model is evaluated on the testing set using the following metrics:

* **Accuracy**: The percentage of loans that are correctly classified as either risky or not risky.
* **Precision**: The percentage of loans that are predicted to be risky that are actually risky.
* **Recall**: The percentage of risky loans that are correctly predicted as risky.

## Conclusion

The deep learning model achieved an accuracy of 75% on the testing set. This indicates that the model is able to predict the risk of student loan default with a reasonable degree of accuracy.

## Further Work

There are a number of ways to improve the performance of the model. Some possible improvements include:

* Trying different model architectures, such as convolutional neural networks or recurrent neural networks.
* Tuning the hyperparameters of the model, such as the learning rate, the number of epochs, and the number of hidden layers.
* Adding more features to the dataset, such
