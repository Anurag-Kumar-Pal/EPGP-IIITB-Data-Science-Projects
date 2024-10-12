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
> Your goal is to create an innovative feature for the smart TV platform. This feature aims to accurately identify and interpret five distinct gestures executed by users, facilitating television control without the need for a traditional remote.

##### **Dataset**:
> - The training data consists of a few hundred videos categorized into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images).
> - The videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos).
> - Sample Images from “Thumbs Up” folder:
> ![image](https://github.com/user-attachments/assets/f9643728-b8d6-4072-9882-f9ee07735e08)




## Libraries Used

- Pandas
- NumpPy
- Matplotlib
- Tensorflow
- Keras 
- Glob
- Os
- Datetime
- Cv2
- Imageio
- Random
- Logging

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
