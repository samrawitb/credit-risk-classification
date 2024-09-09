# credit-risk-classification

1. Overview of the Analysis
   
The purpose of this analysis is to evaluate the performance of a logistic regression model in predicting loan statuses. The model was trained to classify loans as either '0' (healthy loan) or '1' (high-risk loan). This analysis aims to assess the model’s accuracy, precision, and recall, and provide recommendations on whether the model is suitable for deployment in production for use by the company.

2. Results

•Accuracy Score: 99%
The model correctly predicted the loan status in 99% of the cases in the test set, demonstrating high overall accuracy.

•Precision (for high-risk loans '1'): 0.98
The model's precision indicates that when it predicts a loan as high-risk, it is correct 98% of the time. This reduces the chances of false positives (i.e., labeling healthy loans as high-risk).

•Recall (for high-risk loans '1'): 0.87
The recall score shows that the model correctly identifies 87% of actual high-risk loans. This means 13% of high-risk loans were missed by the model (false negatives).


3. Summary
   
The logistic regression model performed exceptionally well on the '0' (healthy loan) class, with near-perfect accuracy and precision. However, it demonstrated slightly lower recall for the '1' (high-risk loan) class, likely due to the class imbalance in the data (more healthy loans than high-risk loans).

Recommendation:

I recommend using this model for production, with the caveat that the recall for high-risk loans can be improved. The model’s high precision means that when it flags a loan as high-risk, it is very likely correct, which is valuable for minimizing unnecessary interventions. However, the slightly lower recall suggests that some high-risk loans might be missed. This could be mitigated by exploring techniques such as:

•	Oversampling the minority class (high-risk loans).
•	Adjusting the decision threshold to increase recall for high-risk loans.
•	Trying more advanced machine learning models, such as Random Forest or Gradient Boosting.

Overall, this model provides strong performance, especially in identifying healthy loans, and is a solid candidate for deployment with some additional tuning to reduce false negatives.
