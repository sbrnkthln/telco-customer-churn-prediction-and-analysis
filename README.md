# Telco Customer Churn Prediction and Analysis
**This project aims to predict customer churn and analyze the factors contributing to it, enabling strategic resource allocation. By identifying customers at high risk of leaving and understanding the key drivers of their churn, the company can implement targeted retention strategies.**

**Problem Statement:** <br/>
The company wants to identify which customers are likely to churn in the future and understand the factors that cause customers to churn, as the company aims to allocate marketing costs carefully to save on marketing expenditures, since revenue is also a major concern.

**Objectives Analysis/Goals:** <br/>
To build a machine learning model that can identify customers likely to churn and analyze the factors that cause customers to churn. This aims to enable the company to allocate time and resources effectively and efficiently.

**Target:** <br/>
1 (Positive): Customer churn
0 (Negative): Customer tidak churn

**Analytic Approach:** <br/>
Analyze the data, then select and build a classification machine learning model that can predict customers likely to churn.

**Metric Evaluation:** <br/>

- Type 1 error (False Positive):
Interpretation: Incorrectly predicting that a customer will churn (when they actually will not churn).
Consequence: Financial loss due to offering special deals to customers who are not actually at risk of churning.

- Type 2 error (False Negative):

Interpretation: Incorrectly predicting that a customer will not churn (when they actually will churn).
Consequence: Loss of customers due to not offering special deals to customers who are actually at risk of churning.
Given the company's problem, the model built must minimize Type 2 error (False Negative), because losing customers incurs a higher cost compared to the cost of offering special deals. In other words, errors resulting from FN (losing customers) are more detrimental than FP (incurring the cost of special offers).

As for the metric, ROC AUC is chosen as the main metric because the model can be threshold-tuned to achieve an optimal balance between True Positive Rate (Recall) and False Positive Rate, and to adjust the score to best suit the business problem.

Since the main goal in this case is to minimize the loss of customers (False Negatives), the modeling will focus on achieving a high Recall score to minimize undetected customer loss.
