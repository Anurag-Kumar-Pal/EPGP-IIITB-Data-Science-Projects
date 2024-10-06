# Predicting Telecom Customer Churn using Logistic Regression
> Analyze customer-level data from a leading telecom firm to build predictive models that identify high-risk churn customers.


## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Results](#results)
* [Conclusions](#conclusions)
* [Business Recommendations](#business-recommendations)


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
- Sklearn
- Statsmodels
- Re
- Mlxtend
- SMOTE

## Steps Involved

- Importing the Required Libraries
- Reading the Dataset and Initial Exploration
- Dataset Cleansing and Dataset Transformation before EDA
- Data Preparation
- Null Value Treatement
- Data Visualization and Conducting EDA
- Preparing Data for Model Building
- Model Building (With and Without PCA)
- Model Evaluation
- Constructing the ROC Curve and Evaluating Accuracy
- Calculating Precision and Recall
- Making Predictions on the Test Dataset
- Finding out Feature Importance
- Model Comparisons
- Writing Conclusions
- Providing Recommendations

## Results

> Here’s a list of factors that are the top predictors of customer churn:

![image](https://github.com/user-attachments/assets/af982e09-7f51-40d8-8f39-1f1863d6500b)


##### Modelling without PCA:
> Evaluation Metrics for the Test Dataset || Building a LogisticRegression Model (Without PCA):
> - Accuracy: 0.81
> - Sensitivity: 0.82
> - Specificity: 0.80
> - Precision: 0.29
> - Recall: 0.82


##### Modelling with PCA:
> Accuracy Metrics for Test Set || LogisticRegression Model (With PCA):
> - Accuracy: 0.82
> - Sensitivity: 0.84
> - Specificity: 0.82

> Accuracy Metrics for Test Set || Random Forest Model (With PCA):
> - Accuracy: 0.85
> - Sensitivity: 0.74
> - Specificity: 0.87

> Accuracy Metrics for Test Set || Decision Tree Model (With PCA):
> - Accuracy: 0.83
> - Sensitivity: 0.70
> - Specificity: 0.84

> Modelling with PCA Model Preference
> As we're prioritising Sensitivity over Accuracy, we will choose Logistic Regression Model (With PCA).
> *Reason: Sensitivity Metric: LogisticRegression Model (0.84) > Random Forest Model (0.74) > Decision Tree Model (0.70)*


## Conclusions

##### Conclusion 1 : 
> LogisticRegression Model (With PCA) has a better Training Accuracy (0.82) and Sensitivity (0.84) compared to the LogisticRegression Model (Without PCA) with a Training Accuracy (0.81) and Sensitivity (0.82)

##### Conclusion 2 : 
> As per the problem statement, the main objective of identifying important predictor attributes which help the business understand indicators of churn. Hence, we will go with **"Modelling without PCA"** as it expliains the important predictor variables as well as the significance of each variable.


## Business Recommendations

> 1. Focus on the customers who have a high average Recharge amount in "Good Phase" as there's a higher probability for such customers to Churn.
> 2. Customers having increasing incoming local minutes of usage for operators T to other operator mobiles for the month of July are more likely to churn.
> 3. Customers who are frequently doing recharges of higher amounts in the month of July are more likely to churn.
> 4. Customers who have recharges of lesser amount in the the month of August are more likely to churn.
> 5. Cutomers, whose monthly 2G/3G recharges in the month of August is high, are more likely to be churn.
> 6. Customers having decreasing total outgoing minutes of voice calls in the month of August are more likely to churn.
> 7. Customers having decreasing local outgoing voice calls in the month of August are more likely to churn.
> 8. Customers for which the recharge amount has been decreasing in the "Action Phase" are more likely to churn.
