# Sales Forecasting for Medicinal Drugs of Rossmann Stores
> Develop a reliable forecasting model using historical sales data from 1,115 Rossmann stores to predict daily sales for the next six weeks.

## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)
* [Business Recommendations](#business-recommendations)


## General Information

##### **Business Understanding**:
> Rossmann is a European drug distributor which operates over 3,000 drug stores across seven European countries. Since a lot of drugs come with a short shelf life, that is, they do not have a long expiry date, it becomes imperative for Rossmann to accurately forecast sales at their individual stores. Currently, the forecasting is taken care of by the store managers who are tasked with forecasting daily sales for the next six weeks. As expected, store sales are influenced by many factors, including promotional campaigns, competition, state holidays, seasonality, and locality. Since the company is just embarking on this project, the scope has been kept to nine key stores across Europe. The stores are key for the company keeping in mind the revenue and historical prestige associated with them. These stores are numbered - 1,3,8,9,13,25,29,31 and 46.


##### **Problem Statement**: 
> With thousands of individual managers predicting sales based on their unique circumstances and intuitions, the accuracy of the forecasts is quite varied. To overcome this problem, the company has hired you as a data scientist to work on the forecasting problem. As part of your job role, you are tasked with building a forecasting model to forecast the daily sales for the next six weeks. To help you with the same, you have been provided with historical sales data for 1,115 Rossmann stores.

##### **Dataset**:
> Dataset has 2 files as explained below: 
> 1. 'store.csv' contains the metadata for every single store.
> 2. 'train.csv' contains the sales data for individual stores at a daily level along with the details about the day.


## Libraries Used

- Pandas
- NumpPy
- Matplotlib
- Seaborn
- Sklearn
- Statsmodels

## Steps Involved

- Importing the Required Libraries
- Reading the Dataset and Initial Exploration
- Dataset Cleansing and Dataset Transformation before EDA
- Data Visualization and Conducting EDA
- Feature Engineering
- Time Series Analysis
- Dividing the Data into Training and Testing Sets
- Model Building
- Model Evaluation
- Model Selection
- Predicting for the next 6 weeks (1st Aug 2015 to 11th September 2015)
- Writing Conclusions
- Providing Recommendations

## Results

##### 1. Summary of all the forecasting models that have been built:
   
![image](https://github.com/user-attachments/assets/12407678-dd27-48bc-85cc-e1cfff478aa9)


##### 2. Here’s a plot of the forecasts of VAR model:
   
![image](https://github.com/user-attachments/assets/eb59804f-6452-40d0-bab1-3d79322c1055)


##### 3. Here’s a plot of the Train and "var_newweeks_forecast" for the next 6 weeks (1st Aug 2015 to 11th September 2015):
   
![image](https://github.com/user-attachments/assets/1491426a-dd3d-4381-a0da-c1280fd7b37c)




## Conclusions

##### Positive Correlation (Directly Related):
> - "AMT_GOODS_PRICE" is positively correlated to "LOAN_AMT_LAKHS"
> - "AMT_ANNUITY" is positively correlated to "LOAN_AMT_LAKHS"
> - "APPLICANT_AGE" shows positive correlation with "YEARS_OF_EMPLOYMENT", "DAYS_REGISTRATION" and "DAYS_ID_PUBLISH"


##### Negative Correlation (Inversely Related):
> - "FLAG_EMP_PHONE" is negatively correlated to "YEARS_OF_EMPLOYMENT" and "APPLICANT_AGE"
> - "HOURS_APPR_PROCESS_START" shows negative correlation with "REGION_RATING_CLIENT" and "REGION_RATING_CLIENT_W_CITY"
