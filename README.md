# credit-risk-classification

Overview of the Analysis
In this analysis, the goal was to build a model to assess the creditworthiness of borrowers using historical lending data. The dataset provided information on various financial attributes of borrowers, and the task was to predict whether a loan is considered high-risk or healthy.

The analysis followed the following stages:

-Splitting the data into training and testing sets.
-Creating a logistic regression model using the original data.
-Predicting loan status using a logistic regression model trained on resampled training data.
-Writing a credit risk analysis report. The logistic regression model was used as the machine learning algorithm, and resampling techniques were -applied to address the imbalanced nature of the data.

Results

Machine Learning Model 1: The logistic regression model using the original data achieved a balanced accuracy score of 95.2%. However, when examining the precision, it performed poorly in predicting high-risk loans (label 1) with only 85% precision. This suggests that the model is better at predicting healthy loans (label 0) than identifying high-risk loans.

Classification Report:

-Precision for healthy loans (label 0): 100%
-Precision for high-risk loans (label 1): 85%
-Recall for healthy loans (label 0): 99%
-Recall for high-risk loans (label 1): 91%

Machine Learning Model 2: The logistic regression model trained on oversampled data showed improved results compared to the original data model. The balanced accuracy score improved at 99.4%. The precision for high-risk loans increased to 99%, indicating a significant improvement in identifying high-risk loans.

Classification Report:

-Precision for healthy loans (label 0): 100%
-Precision for high-risk loans (label 1): 99%
-Recall for healthy loans (label 0): 99%
-Recall for high-risk loans (label 1): 99%

Summary

Based on the results, the logistic regression model trained on oversampled data (Machine Learning Model 2) outperformed the original data model. It showed higher precision and recall for high-risk loans, which is crucial in identifying potential credit risks.

When assessing loan risk, it is more important to have high precision for high-risk loans (label 1) to minimize the chances of misclassifying loans with higher default probabilities. Machine Learning Model 2 demonstrated a significant improvement in this aspect.

Therefore, it is recommended to use Machine Learning Model 2 for credit risk assessment, as it provides better performance in identifying high-risk loans and offers more accurate predictions for creditworthiness analysis.