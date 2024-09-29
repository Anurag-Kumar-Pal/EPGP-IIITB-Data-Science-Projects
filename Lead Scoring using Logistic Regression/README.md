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
> An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%. Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. A typical lead conversion process can be represented using the following funnel:

![image](https://github.com/user-attachments/assets/5473d5b0-ef37-4025-83d8-ee0d67fbf530)



##### **Problem Statement**: 
> X Education aims to improve its lead conversion strategy by developing a predictive model that assigns lead scores, indicating the likelihood of converting prospects into paying customers. With a target conversion rate of 80% set by the CEO, the challenge is to analyze existing data and identify key factors to prioritize leads effectively, enhancing overall sales performance.


##### **Dataset**:
> Dataset has 3 files as explained below: 
> 1. "Leads.csv" contains 37 columns and 9240 rows of lead scoring data.
> 2. "Leads Data Dictionary" contains Leads data variables and its descriptive part.
> 3. "Assignment Subjective Questions" contains four subjective question of Lead Scoring analysis and looking for its outcome.

## Libraries Used

- Pandas
- NumpPy
- Matplotlib
- Seaborn

## Steps Involved

- Importing Libraries
- Reading the Dataset and Initial Exploration
- Dataset Cleansing and Dataset Transformation before EDA
- Handling Missing Values in the Dataset
- Data Visualization and Conducting EDA
- Preparing Data for Model Building
- Dividing the Data into Training and Testing Sets
- Feature Scaling
- Model Building
- Model Evaluation
- Constructing the ROC Curve and Evaluating Accuracy
- Calculating Precision and Recall
- Making Predictions on the Test Dataset
- Assigning Lead Score
- Finding out Feature Importance
- Conclusions

## Results

##### 1. Plotting ROC Curve:
- Area under curve (auc) is approximately 0.88; close to ideal auc of 1

![image](https://github.com/user-attachments/assets/9103491f-7b99-4616-83b6-eb4900706901)

##### 2. Plotting Accuracy, Sensitivity and Specificity:
- 0.4 is the optimum point to take as a cutoff probability.
  
![image](https://github.com/user-attachments/assets/9137b263-02a8-41e9-84a6-2a8f30a69023)


##### 3. Plotting the Feature Importance Graph:

![image](https://github.com/user-attachments/assets/6749262e-6a76-4756-9969-d163946050ae)

##### 4. Evaluation Metrics for the Train Dataset:
- Accuracy: 0.81
- Sensitivity: 0.70
- Specificity: 0.88
- Precision: 0.78
- Recall: 0.70
- Positive predictive value: 0.78
- Negative predictive value: 0.82


##### 5. Evaluation Metrics for the Test Dataset:
- Accuracy: 0.81
- Sensitivity: 0.75
- Specificity: 0.84
- Precision: 0.73
- Recall: 0.75
- Positive predictive value: 0.73
- Negative predictive value: 0.86


## Conclusions

##### Features having Positive Impact on Conversion pPobability in Decreasing Order of Impact:
> - Lead Origin_Lead Add Form
> - Last Activity_Had a Phone Conversation
> - What is your current occupation_Working Professional
> - Lead Source_Welingak Website
> - Last Notable Activity_Unreachable
> - Lead Source_Olark Chat
> - Last Activity_SMS Sent
> - Total Time Spent on Website


##### Features having Negative Impact on Conversion Probability in Decreasing Order of Impact:
> - Lead Profile_Student of SomeSchool
> - Do Not Email
> - Last Activity_Olark Chat Conversation
