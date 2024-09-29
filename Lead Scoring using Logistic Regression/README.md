# Predictive Lead Scoring using Logistic Regression
> Develop a logistic regression model to assign a lead score ranging from 0 to 100 for each lead, enabling the company to effectively target high-potential leads.

## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> The loan providing companies find it hard to give loans to the people due to their insufficient or non-existent credit history. Because of that, some consumers use it to their advantage by becoming a defaulter. When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
> - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
> - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.


##### **Problem Statement**: 
> X Education aims to improve its lead conversion strategy by developing a predictive model that assigns lead scores, indicating the likelihood of converting prospects into paying customers. With a target conversion rate of 80% set by the CEO, the challenge is to analyze existing data and identify key factors to prioritize leads effectively, enhancing overall sales performance.


##### **Dataset**:
> Dataset has 3 files as explained below: 
> 1. 'application_data.csv' contains all the information of the client at the time of application.
The data is about whether a client has payment difficulties.
> 2. 'previous_application.csv' contains information about the client’s previous loan data. It contains the data on whether the previous application had been Approved, Cancelled, Refused or Unused offer.
> 3. 'columns_description.csv' is data dictionary which describes the meaning of the variables.


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
