# Predicting Telecom Customer Churn using Logistic Regression
> Analyze customer-level data from a leading telecom firm to build predictive models that identify high-risk churn customers.


## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition. For many incumbent operators, *retaining high profitable customers is the number one business goal.* To reduce customer churn, **telecom companies need to predict which customers are at high risk of churn.** There are two main models of payment in the telecom industry - postpaid (customers pay a monthly/annual bill after using the services) and prepaid (customers pay/recharge with a certain amount in advance and then use the services).
> - In the postpaid model, when customers want to switch to another operator, they usually inform the existing operator to terminate the services, and you directly know that this is an instance of churn.
> - However, in the prepaid model, customers who want to switch to another network can simply stop using the services without any notice, and it is hard to know whether someone has actually churned or is simply not using the services temporarily (e.g. someone may be on a trip abroad for a month or two and then intend to resume using the services again).

> Thus, churn prediction is usually more critical (and non-trivial) for prepaid customers, and the term ‘churn’ should be defined carefully.  Also, prepaid is the most common model in India and Southeast Asia, while postpaid is more common in Europe in North America.


##### **Problem Statement**: 
> The goal of this project is to predict customer churn in the ninth month by utilizing data collected from the first three months. To achieve accurate predictions, it is essential to gain insights into typical customer behavior associated with churn.

##### **Dataset**:
> Dataset has 3 files as explained below: 
> 1. 'telecom_churn_data.csv' The dataset contains customer-level information for a span of four consecutive months - June, July, August and September. The months are encoded as 6, 7, 8 and 9, respectively. 
> 2. 'Data Dictionary - Telecom Churn.xlsx' contains the data dictionary contains meanings of abbreviations. Some frequent ones are loc (local), IC (incoming), OG (outgoing), T2T (telecom operator to telecom operator), T2O (telecom operator to another operator), RECH (recharge) etc. The attributes containing 6, 7, 8, 9 as suffixes imply that those correspond to the months 6, 7, 8, 9 respectively.

## Libraries Used

- Pandas
- NumpPy
- Matplotlib
- Seaborn

## Steps Involved

- Reading the datasets
- Deleting the columns that are not required
- Null Value Treatement
- Data Sanity Checks
- Removing Outliers
- Creating new Categorical and Numerical columns for better analysis
- Peforming Univariate Analysis On The Data
- Performing Univariate Analysis for Continuous Variables
- Performing Bi-Variate Analysis
- Performing Multi-Variate Analysis
- Merging both the dataframes ("previous_application" and "application_data") and performing analysis again
- Performing Bi-Variate Analysis on the Merged Dataframe
- Performing Multi-Variate analysis on the merged dataframe
- Deriving Inferences after completion of the EDA
- Writing Conclusions

## Results

> Here’s a heatmap that illustrates the linear correlations among various factors for applicants who defaulted on their loans:

![image](https://github.com/user-attachments/assets/e5086564-28ba-42e2-8c37-17128c7bf186)


## Conclusions

##### Positive Correlation (Directly Related):
> - "AMT_GOODS_PRICE" is positively correlated to "LOAN_AMT_LAKHS"
> - "AMT_ANNUITY" is positively correlated to "LOAN_AMT_LAKHS"
> - "APPLICANT_AGE" shows positive correlation with "YEARS_OF_EMPLOYMENT", "DAYS_REGISTRATION" and "DAYS_ID_PUBLISH"


##### Negative Correlation (Inversely Related):
> - "FLAG_EMP_PHONE" is negatively correlated to "YEARS_OF_EMPLOYMENT" and "APPLICANT_AGE"
> - "HOURS_APPR_PROCESS_START" shows negative correlation with "REGION_RATING_CLIENT" and "REGION_RATING_CLIENT_W_CITY"
