Credit-risk-classification analysis


This analysis aimed to determine if the loans labeled healthy/not healthy were labeled correctly. There was data on the loan size, interest rate, debt to income, number of accounts, derogatory marks, and total debt. All this data was put into the model and the algorithm determined if the loan was risky or safe. Safe loans were labeled with a 0, while risky loans were a 1. 

We divided the data into independent and dependent variables. The dependent variable (y) was the loan quality or loan_status since it relies on the other information. The rest of the values were our independent variables (x) which I kept in a DataFrame. We split data into training and testing data to train the model and then fit the model into the training data by instantiating the Logistic Regression Model. 

Finally, I created a 'results' DataFrame with the model's predictions and the results (loan_status) from the original data. To evaluate the models' accuracy, I created a confusion matrix. The categories were 'healthy_loan' and 'high_risk_loan'.

The results were positive. The biggest risk is a false positive because the model would state that the borrower is creditworthy when they are not. This is a huge risk for the lender. Luckily the precision (True Positives/True Positives + False Positives) was 100 percent meaning there were no false positives for healthy loans. There were some false positives for high-risk loans, around 15 percent, which could lead to lost opportunities, but the support (sample size) was much lower. When you factor in the amount of support using a weighted average, the accuracy increases from 85 percent to 99 percent. 

I would recommend this model due to the low amount of False Positives for healthy loans. This means that the model is low risk. 
