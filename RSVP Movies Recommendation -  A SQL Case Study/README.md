# Providing Movie Recommendations using SQL
> Use SQL to analyse the given movie data and give recommendations to RSVP Movies based on the insights.

## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> RSVP Movies is an Indian film production company which has produced many super-hit movies. They have usually released movies for the Indian audience but for their next project, they are planning to release a movie for the global audience in 2022.The production company wants to plan their every move analytically based on data and have approached you for help with this new project.

##### **Problem Statement**: 
> Analyze movie data using SQL to identify insights on box office performance and provide actionable recommendations for RSVP Movies to improve film selection and marketing strategies.

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
