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

##### 1. Below is the executive summary of the experiments carried out to identify the optimal model for the given problem statement:

![image](https://github.com/user-attachments/assets/3e8f2ee9-43ea-4ac2-9258-144adf21d441)

##### 2. Model #11: Graph of Model Accuracy and Model Loss

![image](https://github.com/user-attachments/assets/6393fd93-fbf0-48c3-9ccc-7032161e34ea)



## Conclusions

##### Model Selection Results

> - Selected Model: Model 11 Transfer Learning With GRU and Training all Weights
> - Reason: This model has been selected as it has the best training and validation accuracies.
> - Training Accuracy: 99%
> - Validation Accuracy: 99%
> - File Name: model-00013-0.02487-0.99548-0.03481-0.99000.h5
