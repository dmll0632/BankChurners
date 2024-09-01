# Bank Churn Prediction Project


## Project Overview

This project focuses on identifying which customers are at risk of churning (i.e., stopping the use of a bank’s services). The main objective is to create and evaluate a predictive model that accurately identifies these customers, allowing the bank to enhance its customer retention strategies.

**Objective**

The primary objective of this project is to build a predictive model that can identify customers at risk of churning. By understanding the factors that contribute to customer churn, the bank can develop more effective strategies to retain its customers and reduce churn rates.

**Steps Involved**

**1. Data Preparation and Exploration**

Data Cleaning:

Address any missing values, outliers, or inconsistencies in the dataset to ensure that the data is ready for analysis.
Remove any duplicate records to prevent skewed results.
Choosing the Dataset:

The dataset chosen for this project is the "Bank Customer Churn" dataset from Kaggle.
The dataset includes various features related to customer demographics, account information, and transaction history.
Feature Engineering:

Transform existing features and create new ones to improve the predictive power of the model.
Examples include deriving customer tenure or aggregating transaction data.
Encoding Categorical Variables:

Apply label encoding to ordinal variables where categories have a meaningful order.
Apply one-hot encoding to nominal variables to convert categorical data into a format that can be provided to ML algorithms.
Normalization and Scaling:

Normalize the features to ensure that all features contribute equally to the model.
Apply scaling techniques like StandardScaler or MinMaxScaler to bring all features to a similar scale, which is particularly important for distance-based models.
Feature Selection:

Use statistical methods or algorithms to select the most relevant features for the model.
Reduce dimensionality to avoid overfitting and improve model performance.


**2. Model Building**


Several machine learning algorithms were considered for this project:

K-Nearest Neighbors (KNN):

A simple, instance-based learning algorithm where the class of a sample is determined by the majority class among its k-nearest neighbors.
Logistic Regression:

A linear model used for binary classification problems, predicting the probability of a customer churning.
Decision Trees:

A non-linear model that splits the data into branches based on feature values to make predictions. This model is easy to interpret and can capture complex relationships in the data.
Bagging:

An ensemble method that combines multiple models (typically decision trees) trained on different subsets of the data to reduce variance and improve robustness.
Pasting:

Similar to bagging, but instead of using sampling with replacement, pasting uses sampling without replacement to create different subsets of the training data for model training.
Random Patches:

Extends bagging by sampling both instances and features. This technique is useful for high-dimensional data and helps reduce overfitting by encouraging diversity in the models.
AdaBoost:

An ensemble method that focuses on creating a strong classifier by sequentially correcting the errors of previous models. It assigns higher weights to misclassified instances in subsequent iterations.
Gradient Boosting:

Another ensemble technique that builds models sequentially, where each new model corrects the errors of the previous one. It is highly effective for both regression and classification tasks and is known for its accuracy.
3. Model Evaluation and Testing
Split the dataset into training and testing sets to evaluate the model's performance on unseen data.
Use metrics such as accuracy, precision, recall, F1-score, and ROC-AUC to assess model performance.
Perform cross-validation to ensure that the model generalizes well to new data.
4. Ensemble Techniques for Enhanced Prediction
In addition to individual models, ensemble techniques like Bagging, Pasting, Random Patches, AdaBoost, and Gradient Boosting were used to improve prediction accuracy and model robustness. These methods combine multiple models to reduce the risk of overfitting and increase generalization performance.



**Conclusion**

This project provides insights into the factors that lead to customer churn and offers a predictive model that the bank can use to identify at-risk customers. By leveraging these insights and advanced modeling techniques, the bank can take proactive measures to retain customers and reduce churn rates, ultimately improving customer satisfaction and loyalty.
