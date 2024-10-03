# Forecasting Bike Sharing Demand with Linear Regression Analysis
> Build a multiple linear regression model to forecast the demand for shared bikes.


## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system. A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
> In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


##### **Problem Statement**: 
> Suppose you work for a consumer finance company that specializes in providing various loan types to urban customers. Your task is to conduct exploratory data analysis (EDA) to identify patterns in the data, ensuring that applicants who are capable of repaying their loans are not unfairly rejected.

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
