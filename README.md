# credit-risk-classification

Overview of the Analysis:
The purpose of this analysis is to create a machine learning model that would allow users to predict whether or not a loan is "Healthy" or "HIgh-Risk" based on the characteristics of the borrower. The data used to create and train the machine learning model included the following information: the loan amount, the interest rate on the loan, the borrower's income, their debt-to-income ratio, number of accouts, derogatory remarks on the accounts, and total debt. The data also provided the loan status - whether the loans were "healthy" (0) or "high-risk" (1).

The dataset provided had many more "healthy" loans than "high-risk" loans (75,036 vs. 2500 respectively).

Results
- Precision Scores
  - "healthy": 1.00
  - "high-risk": 0.85
- Recall Scores
  - "healthy": 0.99
  - "high-risk": 0.91
 
Summary:
The model has a high accuracy score which is indicative of a well predicting model. The very high precision and recall values for '0' labels indicate that the model predicts healthy loans very well. The precision and recall values for '1' labels is poorer, indicating that the high-risk loans are not categorized as well. This potentially is due to our model being trained with data that has significantly more '0' samples.

A way to counteract this would be to create new random samples that have an equal number of smaples for both labels and train another model.

For the purpose of this application, it is more important for a company to correctly classify high-risk loans than healthy loans. Loans that default (aka high-risk) would cost the company the entire principal amount of the loan. Whereas incorrectly labeling a healthy loan as high-risk would only lead to a potential loss of profit from missed interest payments. 

I would not recommend this model becuase of the skew in more '0' labeled samples. A model trained with an even number of samples would be ideal.
