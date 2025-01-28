# Telecom Churn Analysis
In this project, we are going to explore an IBM sample dataset--Telco customer churn data, where Telco is a fictional telecom company providing internet and phone services. The dataset refers to the Q3 customers (7043 unique instances in total).

Although IBM has provided multiple Excel files of data with demographics, location, population, services and status, the dataset we used is preprocessed by [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data) creators. See details below for information. 
## Executive Summary
Feel free to play with the interactive version of dashboard through [Tableau](https://public.tableau.com/app/profile/irene.shi2071/viz/TelecomChurnCustomerAnalysis/ChurnCustomerAnalysis)!
![Figure 1](<Churn Customer Analysis.png>)

## Insights Deep-Dive
### Demographics
Within 7043 customers in Q3, there are 1869 (27%) of churn customer whose monthly charges have $139k in total and $74.44 on average. Based on demographic features, there's only slight gender difference (0.4%); 25% of churn customers are senior citizen; meanwhile, the majority of them are without partner (61%) or dependent (83%). 

### Account/Payment Info
From account-wise perspective, churn happens the most among less than 6 months subscription (42%) and more than half of them deployed Electronic check for payment. It turns out 89% of churn customers (1655) are using month-to-month contract. 

Based on the relationship between monthly chages and tenure, we can see that there's a slightly positive trend, indicating the customers with high monthly charges are likely to transform to churn over time.

### Service Type
As for service types, there are two categories--phone and internet. Among all internet services, churn customers without services of online backup, online security, device protection, and tech support are at least 36% more than those using these services, whereas in streaming movies and streaming tv, there are a fewer discrepancy between the two groups of people.

91% of churn users are equipped with phone services. Meanwhile, half proportion of those users are using multiple lines services and the other half are not, indicating the `multiple line` service feature a weak estimator for prediction of churn.

However, for both categories of services, active users tend to have more even distribution of the usage of different kind of services. With more specific correlation matrix, the features such as `online backup`, `online security`, `device protection`, and `tech support` can be used for modeling.

