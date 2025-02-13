Loan Default Risk prediction using SAS
Introduction
Machine learning is used to analyze loan default by applying algorithms to forecast the probability of borrowers failing to repay their debts. This predictive modeling technique uses past data such as credit histories of debtors, repayment trends as well as additional financial indicators. Machine learning algorithms can detect possible default risks by examining patterns and correlations in the data. Financial institutions use this information to make well-informed lending decisions, efficiently manage risk as well as minimize losses. This analytical technique improves conventional credit scoring by integrating more types of data points and complicated nonlinear correlations.
Problem Statement
•	The research will use SAS to analyze the information in order to identify patterns that differentiate consumers who fail on loans from those who do not.
•	The model involves building predictive models using SAS to estimate future occurrences of loan defaults based on the chosen characteristics.
•	The model involves using Tableau to develop interactive dashboards that visually represent the distinguishing features of individuals who default on loans compared to those who do not as well as the influence of collections on loan repayments.
About the Data
The dataset contains customers who have fully repaid their loans customers who have defaulted and been sent to collections without repaying their debts and collecting interest and customers who have only repaid their loans after being sent to collections. The initial dataset has 113,937 rows and 81 columns from which 12 particular features were chosen for analysis. A total of 871 data points were excluded from the study owing to variations or missing information. 
Reference
https://www.kaggle.com/datasets/nurudeenabdulsalaam/prosper-loan-dataset?select=prosperLoanData.csv
Tableau Visualizations and Interpretation of Findings
 
Interpretation
There are higher customers who are income verified and loan is running. The customers who completed loan are also relatively higher who are income verified. Since the data is imbalanced, the findings cannot be accurate. Hence, finding the ratio based on income verified customers can be more precise that can be measured in same scale.


 
Interpretation
In credit grade HR, the default rate is higher and the completion rate is higher in Grade C credit. Also, the chargedoff loans are relatively higher in credit grade D. This shows based on credit grade, loan defaulters can be predicted as in HR grade, the default rate is higher. Banking companies can focus on such customers with such credit grade.
 
Interpretation
The table shows there are higher customers whose loans are existing which fall in other occupation categories. These customers do not have specific occupation. Such customers can be scanned with proper documents related to their income to flag defaulters as the default rate is higher in this category.
 
Interpretation
The customers who are having higher borrower rate related delayed their payment of more than 120 days. The customers who defaulted have relatively lower borrower rate. This shows customers with higher borrower rate are most likely to delay the loan payments which can be disruptive for banking sectors.
 
Interpretation
The APR (Annual Percentage Rate) rate of borrower is higher of customer who delayed payments more than 120 days. Also, the customer who paid on time had lower APR. This plot is helpful for promptly evaluating the distribution of loan statuses in a portfolio and pinpointing regions that may need attention because of increased risk.
 
Interpretation
The plot shows that customers who has existing loans, defaulted or having payments due in 16 to 30 days are having higher average current credit lines. The banks can screen customers based on number of current credit lines where customers who default the loans might have higher current credit lines.
 
Interpretation
The debt to income ratio is another financial indicator that can help to screen defaulters where the treemap shows that customers who are past due in 60 to 90 days have higher debts based on income. Customers who had lower debts also cancel the loans which can be alarming for banking sector to offer loans to such customers.
Data Exploration and Preprocessing
1.	Missing Data
  
The variables are imported in Python and are also explored in Python. There are lot of missing values in the data which will be imputed either by mean or median imputation approaches. 
2.	Inconsistent Data
The data is consistent but some columns like “ListingKey”,”ListingNumber”, “GroupKey”,”LoanKey” are some columns that are irrelevant. Such columns will be removed.
3.	Reduction of Data
The data has a total of 81 variables where multicollinear variables will be removed which can lead to data leakage. The non collinear variables will be kept in the final analysis with limited variables and imputed observations.
