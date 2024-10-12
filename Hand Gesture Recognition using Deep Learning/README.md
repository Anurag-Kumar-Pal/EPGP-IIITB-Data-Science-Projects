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

- Importing the Required Libraries
- Reading the Dataset and Initial Exploration
- Defining the first "Generator" function
- Model Building
- Model Evaluation
- Model Selection

## Results

> Below is the executive summary of the experiments carried out to identify the optimal model for the given problem statement:
![image](https://github.com/user-attachments/assets/9592bc69-64b2-451f-a501-fabd9591b3b1)





## Conclusions

##### Positive Correlation (Directly Related):
> - "AMT_GOODS_PRICE" is positively correlated to "LOAN_AMT_LAKHS"
> - "AMT_ANNUITY" is positively correlated to "LOAN_AMT_LAKHS"
> - "APPLICANT_AGE" shows positive correlation with "YEARS_OF_EMPLOYMENT", "DAYS_REGISTRATION" and "DAYS_ID_PUBLISH"


##### Negative Correlation (Inversely Related):
> - "FLAG_EMP_PHONE" is negatively correlated to "YEARS_OF_EMPLOYMENT" and "APPLICANT_AGE"
> - "HOURS_APPR_PROCESS_START" shows negative correlation with "REGION_RATING_CLIENT" and "REGION_RATING_CLIENT_W_CITY"
