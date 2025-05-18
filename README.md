# EDA-Report
Capstone Project 20.1: Initial Report and Exploratory Data Analysis (EDA)

**Author:** Christian Daniel Guerra Maraza

#### Executive summary

#### Rationale
It is important because retaining customers is important to keep generating revenues to the bank. If the bank knows what customers will churn it can deploy tactic actions to avoid churn before customers left the bank.

#### Research Question
How can I identify the customers that are going to churn or are more likely to churn the Bank?

#### Data Sources
https://www.kaggle.com/api/v1/datasets/download/saurabhbadole/bank-customer-churn-prediction-dataset?dataset_version_number=2

#### Methodology
The present EDA will be use to generate Logistic regression, SVM and Random Forest models.

#### EDA Insights

<img width="1729" alt="Screenshot 2025-05-18 at 3 10 19 pm" src="https://github.com/user-attachments/assets/d8927392-15e9-4787-9b44-2f8ea4869cd5" />

- Outliers are identified in CreditScore, Age and Number Of Products.
- The majority of customers have an acceptable Credit Scoring, mainly between 600 and 700.
- Customer age is commonly between 30 and 45 years old. The younger ones are 20 years old.
- The bank doesn't have many products, the maximum is 4 products but the average number of products is 1.
-----
 <img width="1516" alt="Screenshot 2025-05-18 at 3 10 31 pm" src="https://github.com/user-attachments/assets/c02caa4d-84e4-436f-9774-09953e375a26" />

 - There is no much older people in the Age distribution, so the bank is focused in the most productive people of the countries.
 - Seems to be an error in Balance variable, due to zero balance in an important number of accounts.
 - Product penetration is low, a few customers have more than 2 products.
-----
<img width="512" alt="Screenshot 2025-05-18 at 3 13 41 pm" src="https://github.com/user-attachments/assets/07496697-f3c0-4515-93ae-177a167b58cf" />

- This dataset has a 20% of churned customers (this is the target variable) so it could be said that the dataset is umbalanced.
-----
<img width="789" alt="Screenshot 2025-05-18 at 3 13 53 pm" src="https://github.com/user-attachments/assets/49d7d465-1db2-4cfd-bf1f-7e6dd1633c39" />

- Proportions of the Credit Score groups are very similar across countries. The Credit policy of the bank must be the same in all countries.
-----
<img width="1194" alt="Screenshot 2025-05-18 at 3 14 40 pm" src="https://github.com/user-attachments/assets/fa7b6fc5-013b-449d-963b-2e7a1e106bed" />

- There is more attrition as a ratio (2x) in Germany than the others countries.
- As a ratio, there is a similar level of cardholders accross countries.
- The % of active members is similar in all countries. However Germany has the lower activation ratio.
-----
<img width="1491" alt="Screenshot 2025-05-18 at 3 14 07 pm" src="https://github.com/user-attachments/assets/5a08c2b0-cf63-47a0-9f5b-8347abf3a668" />

- Numeric variables behave similarly among geographies. Only Germany reports a higher Balance distribution than the other countries.
-----
![pairplot](https://github.com/user-attachments/assets/84914a21-f9cc-4682-be0d-38db0f3d399e)

- Seems to be low correlations accross variables.
- Number of products could be an important variable to classify churned customers.
- customers who churned tend to be older than the others that stayed.
- Customers whi churned have an important concentration in 1 products. If customers have 2 products or more they are less likely to churn.
-----
![corr_matriz](https://github.com/user-attachments/assets/ef325859-3cbf-4c69-a41e-25953ac260f1)

- Low correlations were identified between numeric variables.
- The highest correlation found is Number of products vs Balance (-0.38), followed by Number of products vs Credit Score (-0.11)

-----

#### Next steps
Modeling and Model selection using error/accuracy metrics for the comparisson.
