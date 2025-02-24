# Module 12 Report Template

## Overview of the Analysis

In this challenge, machine learning was used to analyze historical lending data, including loan size, interest rate, borrower income, total debt, debt-to-income ratios, number of accounts, and any derogatory remarks, to predict the likelihood of healthy versus risky loan lending. Loan status served as the dependent variable, with the other factors as independent variables. The process involved splitting the data into training and testing sets, fitting a logistic regression model, making predictions, and evaluating the results using a confusion matrix and classification report.

## Results

Machine Learning Model 1:
	• Accuracy: 0.99
	• Precision:
		○ Class 0: 1.00
		○ Class 1: 0.87
	• Recall:
		○ Class 0: 1.00
		○ Class 1: 0.95
	• F1-Score:
		○ Class 0: 1.00
		○ Class 1: 0.91
	• Macro Average:
		○ Precision: 0.94
		○ Recall: 0.97
		○ F1-Score: 0.95
	• Weighted Average:
		○ Precision: 0.99
		○ Recall: 0.99
      ○ F1-Score: 0.99

      
##Summary

Recommendation:
The machine learning model demonstrates high overall performance, with an accuracy of 0.99. However, the evaluation depends on the specific problem at hand:
	1. Predicting Class 0 (Healthy Loans):
		○ The model achieves perfect precision and recall for Class 0, indicating it is excellent at identifying healthy loans without false negatives or false positives.
	2. Predicting Class 1 (Risky Loans):
		○ While the recall for Class 1 is quite high at 0.95, the precision is lower at 0.87. This means the model is fairly good at identifying risky loans but has a slightly higher rate of false positives (predicting a loan as risky when it is not).
Considerations:
	• Importance of Class Prediction: If the primary goal is to ensure that all risky loans are correctly identified (minimizing false negatives), then the model's high recall for Class 1 is beneficial.
	• Trade-offs: If false positives are costly and it's crucial to minimize them, the precision for Class 1 should be improved, or different models/thresholds should be considered.
Overall, this model performs best given its high accuracy and balanced performance metrics. However, the decision to use this model should depend on the relative importance of correctly predicting healthy versus risky loans. If minimizing false positives in risky loans is critical, additional tuning or alternative models might be warranted.

