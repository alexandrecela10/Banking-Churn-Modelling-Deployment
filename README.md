# Banking-Churn-Modelling-Deployment
Modelling customers churn for a Bank. Exploratory Data Analysis, Automated Data Preprocessing, Modelling with Classification and Ensemble Tree models, Error Analysis, Deployment

## Introduction
This readme file provides a summary of a machine learning (ML) project focused on banking churn modelling. The project aimed to address the business problem of identifying potential churners within a banking customer base. Churn refers to customers who are likely to stop using the bank's services in the near future. By predicting churn, the bank can proactively engage with these customers and take necessary actions to retain them.

## Project Overview
Business Problem Statement
The primary objective of this project was to develop a machine learning model that accurately predicts churn within the bank's customer base. The model would assist the bank in identifying customers who are at a high risk of leaving, enabling proactive measures to be taken to prevent churn.

## Automated Exploratory Data Analysis
To gain insights into the data and understand the characteristics of potential churners, an automated exploratory data analysis (EDA) was performed. The EDA process utilized the Dataprep package along with custom functions. Which you can find in a given repository. This automated approach allowed for efficient data exploration, identification of trends, and understanding the underlying patterns related to churn.

## Automated Data Preprocessing and Modelling with Pipelines
To streamline the data preprocessing and modelling stages, an automated pipeline approach was employed. This pipeline encompassed data preprocessing steps such as feature scaling, handling missing values, and encoding categorical variables. The pipeline further integrated the ML model training and evaluation steps.

## Baseline Models
To establish a baseline for performance comparison, two initial models were trained: L2 logistic regression and a decision tree. These models achieved a recall of 73% and an F1 score of 57%. The baseline models provided a starting point to assess the performance of subsequent models.

## Model Evaluation through Cross-Validation
Multiple models were tested using a five-fold cross-validation approach. This technique involved splitting the data into five subsets and training models on different combinations of these subsets. The performance of each model was evaluated using appropriate metrics such as accuracy, precision, recall, and F1 score. Models tested in this project included Random Forest, Extra Trees Classifier, and XGBoost.

## Automated Hyperparameter Tuning
The best performing model, Extra Trees Classifier, underwent further improvement through hyperparameter tuning. Random Search CV and GridSearch CV techniques were employed to automatically search through a range of hyperparameters and find the optimal combination that improved model performance. This automated process saved time and ensured the best possible configuration was obtained for the model.

## Model Improvement and Error Analysis
Error analysis techniques were utilized to gain a deeper understanding of the model's shortcomings and areas for improvement. By analyzing misclassified instances, the model's weaknesses were identified and addressed. Threshold tweaking techniques were applied to adjust the decision boundary of the model, resulting in an improved F1 score of 60% and recall of 78% on the test set.

## Creation of a List of High Probability Churners
Based on the final model's predictions, a list of customers with a high probability of churning was generated. This list provided the bank with actionable insights, enabling them to prioritize efforts towards retaining these high-risk customers.

## Saving and Deployment of the Final Best Model
Once the best-performing model was identified, it was saved for future use. The final model was deployed in a production environment, allowing the bank to utilize it for real-time churn prediction on new customer data.

## Conclusion
This ML banking churn modelling project successfully addressed the business problem of identifying potential churners within a banking customer base. By automating various stages of the project, including exploratory data analysis, data preprocessing, and hyperparameter tuning, the model achieved a significant improvement in performance. The final best model, an Extra Trees Classifier, demonstrated an F1 score of 60% and a recall of 78% on the
