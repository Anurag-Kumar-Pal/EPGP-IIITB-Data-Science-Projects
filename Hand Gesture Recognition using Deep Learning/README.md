# Hand Gesture Recognition using Deep Learning
> Develop an innovative feature for a smart TV platform that accurately identifies and interprets five distinct user gestures, allowing for intuitive television control without a traditional remote.

## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> You are working as a data scientist at a home electronics company which manufactures state of the art smart televisions.
Your goal is to create an innovative feature for the smart TV platform. This feature aims to accurately identify and interpret five distinct gestures executed by users, facilitating television control without the need for a traditional remote. The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command.
>  - **Thumbs up:**  Increase the volume
>  - **Thumbs down:** Decrease the volume
>  - **Left swipe:** 'Jump' backwards 10 seconds
>  - **Right swipe:** 'Jump' forward 10 seconds
>  - **Stop:** Pause the movie



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
