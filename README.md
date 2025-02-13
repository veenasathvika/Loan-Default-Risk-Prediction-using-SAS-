Loan Default Risk prediction using SAS

Introduction

Machine learning is used to analyze loan default by applying algorithms to forecast the probability of borrowers failing to repay their debts. This predictive modeling technique uses past data such as credit histories of debtors, repayment trends as well as additional financial indicators. Machine learning algorithms can detect possible default risks by examining patterns and correlations in the data. Financial institutions use this information to make well-informed lending decisions, efficiently manage risk as well as minimize losses. This analytical technique improves conventional credit scoring by integrating more types of data points and complicated nonlinear correlations.

Problem Statement

•	The research will use SAS to analyze the information in order to identify patterns that differentiate consumers who fail on loans from those who do not.

•	The model involves building predictive models using SAS to estimate future occurrences of loan defaults based on the chosen characteristics.

•	The model involves using Tableau to develop interactive dashboards that visually represent the distinguishing features of individuals who default on loans compared to those who do not as well as the influence of collections on loan repayments.

About the Data

The dataset contains customers who have fully repaid their loans customers who have defaulted and been sent to collections without repaying their debts and collecting interest and customers who have only repaid their loans after being sent to collections. The initial dataset has 113,937 rows and 81 columns from which 12 particular features were chosen for analysis. A total of 871 data points were excluded from the study owing to variations or missing information. 

References

https://www.kaggle.com/datasets/nurudeenabdulsalaam/prosper-loan-dataset?select=prosperLoanData.csv

Tableau Visualizations and Interpretation of Findings

 ![image](https://github.com/user-attachments/assets/0cf97d74-b4d0-4dad-b1db-4c1b6b032ecc)

Interpretation

There are higher customers who are income verified and loan is running. The customers who completed loan are also relatively higher who are income verified. Since the data is imbalanced, the findings cannot be accurate. Hence, finding the ratio based on income verified customers can be more precise that can be measured in same scale.

![image](https://github.com/user-attachments/assets/3355aab1-5aad-433c-944b-1c0825021c9f)

Interpretation

In credit grade HR, the default rate is higher and the completion rate is higher in Grade C credit. Also, the chargedoff loans are relatively higher in credit grade D. This shows based on credit grade, loan defaulters can be predicted as in HR grade, the default rate is higher. Banking companies can focus on such customers with such credit grade.

 ![image](https://github.com/user-attachments/assets/42087245-2ed5-4ab9-9549-d8e7b207ae67)

Interpretation

The table shows there are higher customers whose loans are existing which fall in other occupation categories. These customers do not have specific occupation. Such customers can be scanned with proper documents related to their income to flag defaulters as the default rate is higher in this category.

 ![image](https://github.com/user-attachments/assets/7e510a92-da51-4025-b184-8d494e3da203)

Interpretation

The customers who are having higher borrower rate related delayed their payment of more than 120 days. The customers who defaulted have relatively lower borrower rate. This shows customers with higher borrower rate are most likely to delay the loan payments which can be disruptive for banking sectors.

 ![image](https://github.com/user-attachments/assets/3aecb359-a513-4b70-8462-9a63b5565322)

Interpretation

The APR (Annual Percentage Rate) rate of borrower is higher of customer who delayed payments more than 120 days. Also, the customer who paid on time had lower APR. This plot is helpful for promptly evaluating the distribution of loan statuses in a portfolio and pinpointing regions that may need attention because of increased risk.

 ![image](https://github.com/user-attachments/assets/5813a873-eb4b-40e7-b6cf-eed799010c57)

Interpretation

The plot shows that customers who has existing loans, defaulted or having payments due in 16 to 30 days are having higher average current credit lines. The banks can screen customers based on number of current credit lines where customers who default the loans might have higher current credit lines.

 ![image](https://github.com/user-attachments/assets/5d3897d6-9684-4e33-ae56-cb89b9cb93eb)

Interpretation

The debt to income ratio is another financial indicator that can help to screen defaulters where the treemap shows that customers who are past due in 60 to 90 days have higher debts based on income. Customers who had lower debts also cancel the loans which can be alarming for banking sector to offer loans to such customers.

Data Exploration and Preprocessing

1.	Missing Data
  
The variables are imported in Python and are also explored in Python. There are lot of missing values in the data which will be imputed either by mean or median imputation approaches. 

![image](https://github.com/user-attachments/assets/daf6d7f0-b819-48cd-abe5-6ff83a45ce9a)
![image](https://github.com/user-attachments/assets/6b208527-628f-456c-b453-01bda44fac7b)


2.	Inconsistent Data
   
The data is consistent but some columns like “ListingKey”,”ListingNumber”, “GroupKey”,”LoanKey” are some columns that are irrelevant. Such columns will be removed.

3.	Reduction of Data
   
The data has a total of 81 variables where multicollinear variables will be removed which can lead to data leakage. The non collinear variables will be kept in the final analysis with limited variables and imputed observations.
