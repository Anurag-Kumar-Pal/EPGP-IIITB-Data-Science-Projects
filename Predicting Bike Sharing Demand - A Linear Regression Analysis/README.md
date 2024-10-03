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
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system. A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

##### **Business Goal**:

> **BoomBikes** has contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
>  - Which variables are significant in predicting the demand for shared bikes.
>  - How well those variables describe the bike demands

##### **Problem Statement**: 
> You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

##### **Dataset**:
> Dataset has 2 files as explained below: 
> 1. 'day.csv' contains the bike sharing data.
> 2. 'Data Dictionary' contains the information of the columns present in the dataset
> - You can observe in the dataset that some of the variables like 'weathersit' and 'season' have values as 1, 2, 3, 4 which have specific labels associated with them (as can be seen in the data dictionary). These numeric values associated with the labels may indicate that there is some order to them - which is actually not the case (Check the data dictionary and think why). So, it is advisable to convert such feature values into categorical string values before proceeding with model building. Please refer the data dictionary to get a better understanding of all the independent variables.
> - You might notice the column 'yr' with two values 0 and 1 indicating the years 2018 and 2019 respectively. At the first instinct, you might think it is a good idea to drop this column as it only has two values so it might not be a value-add to the model. But in reality, since these bike-sharing systems are slowly gaining popularity, the demand for these bikes is increasing every year proving that the column 'yr' might be a good variable for prediction. So think twice before dropping it. 

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
- Removing Unwanted Columns
- Data Visualization and Conducting EDA
- Data Preparation for Multiple Linear Regression Analysis
- Dividing the Data into Training and Testing Sets
- Normalising the Numerical Variables in the Dataset
- Building the Multiple Linear Regression Model via an Iterative Process
- Model Building
- Model Selection
- Prooving of the Assumptions of Linear Regression
- Making Predictions on the Test Data Using the Selected Model
- Model Evaluation
- Mentioning the Predictor Variables and the Equation
- Writing Conclusions

## Results

##### 1. Here’s a heatmap that illustrates the linear correlations among various factors of the bike sharing dataset:
![image](https://github.com/user-attachments/assets/c594bcd5-3e44-457d-af0d-ad5aea935807)

##### 2. Proofs for the assumptions of Linear Regression:
  **Assumption 1:** One crucial assumption posits the existence of a linear relationship between the independent and dependent variables.
  
  ![image](https://github.com/user-attachments/assets/659f1138-883d-422a-b7f4-baa83ab35791)
    
  **Assumption 2:** No auto-correlation i.e, Assumption of Error Terms Being Independent
  
  ![image](https://github.com/user-attachments/assets/307cc96c-58ff-4d45-993f-7a47d3d9a2d7)
    
  **Assumption 3:** No Multicollinearity

  ![image](https://github.com/user-attachments/assets/1f446de5-4d5e-4645-a120-2a73eb3eae2d)
    

  **Assumption 4:** Assumption of Homoscedasticity
  
  ![image](https://github.com/user-attachments/assets/8467c4f2-27dd-40bf-b644-7fa4a2602a66)

  **Assumption 5:** Assumption of Normally Distributed Error Terms
  
  ![image](https://github.com/user-attachments/assets/f08efb94-f245-472d-b609-2af2cc75727f)







## Conclusions

##### Graph actual values of the dataset versus predicted values by the model:

![image](https://github.com/user-attachments/assets/119c4bd3-75e3-4cae-9855-1283cb3b193a)


##### Summary of Training and Test Dataset:

###### Training Dataset:
> - R-squared (R^2): 0.835
> - Adj. R-squared (Adj. R^2): 0.832

###### Testing Dataset:
> - R-squared (R^2): 0.805
> - Adj. R-squared (Adj. R^2): 0.795

##### Demand of the Bikes depend on the following factors:

> - year
> - holiday
> - temp
> - windspeed
> - July
> - Sep
> - Light_Showers
> - Misty
> - Spring
> - Summer
> - Winter

##### Equation of our best-fitted line is:

> - count_of_bike = 0.1994 + (year x 0.2336) - (holiday x 0.0975) + (temp x 0.4910) - (windspeed x 0.1479) - (July x 0.0521) + (Sep x 0.0768) - (Light_Showers x 0.2842) - (Misty x 0.0802) - (Spring x 0.0672) + (Summer x 0.0465) + (Winter x 0.0817)
