# credit-risk-classification

## Kevin Khov

### Overview of the Analysis:
The purpose of this analysis was the create a model that would assist a peer-to-peer lending services company in predicting the creditworthiness of potential borrowers and clients. A dataset of historical lending activity was used the help build this model, and this data included financial information such as loan size, number of accounts, and total debt. The main variable being evaluated for prediction was the "loan status" variable. This variable is valued as either a "0", which represents that the loan is considered healthy, and a "1", which represents that the loan is considered high-risk. Value counts of each were calculated, and the model was evaluated based on its ability to correctly predict if a loan was considered healthy (0) or high-risk (0). The model's value counts were then compared to the actual value counts for the evaluation. As part of this analysis, various stages of the machine learning process were performed. Data was gathered from the dataset into a dataframe and prepared by separating the y and X variables. The data was then split into training and testing datasets, and value counts of each loan type were calculated. The method chosen to be used for this machine learning analysis was Logistic Regression. This method is used to predict the probability that an instance belongs to a given class or not. In this case, it would be if a loan is classified as healthy or high-risk.

### Results:
* Machine Learning Model 1: (Healthy Loan)
  * Precision - 1.00 (did not incorrectly classify any high-risk loans as healthy)
  * Recall - 0.99 (correctly classified almost all healthy loans)
* Machine Learning Model 2: (High-Risk Loan)
  * Precision - 0.84 (mostly did not incorrectly classify any healthy loans as high risk)
  * Recall - 0.94 (correctly classified almost all high-risk loans)
* Overall, model had an accuracy score of 0.99 for predicting both healthy and high-rish loans

### Summary
Overall, both models performed well in predicting the credit worthiness of borrowers. Both models were 99% accurate in predicting when a loan would be classified as "healthy" or "high-risk". However, the model to predict healthy loans performed better than the model to predict high-risk loans as healthy loan model did not incorrectly identify any high-risk loans as healthy with its 1.00 precision score, while the high-risk had a precision score of 0.84, indicating that some errors were made. As we would like to avoid providing loans to borrowers of higher risk, it is more important to correctly predict the high-risk loans. Since the overall accuracy of the models was 99%, I would recommend being able to use both models to predict healthy and high-risk loans.

The code used to create the machine learning model can be found in "credit_risk_classification.ipynb" in the "Credit_Risk" folder. The CSV used to load the data into the model can be found in the "lending_data.csv" file in the "Resources" folder.
