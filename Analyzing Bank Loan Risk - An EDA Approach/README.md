# Identifying Key Factors in Bank Loans using Risk Analysis
> Company wants to identify the key factors contributing to loan defaults to improve its risk assessment and portfolio management.

## Table of Contents
* [General Information](#general-information)
* [Libraries Used](#libraries-used)
* [Steps Involved](#steps-involved)
* [Conclusions](#conclusions)


## General Information

##### **Business Understanding**:
> The loan providing companies find it hard to give loans to the people due to their insufficient or non-existent credit history. Because of that, some consumers use it to their advantage by becoming a defaulter. When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
> - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
> - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

##### **Problem Statement**: 
> Suppose you work for a consumer finance company that specializes in providing various loan types to urban customers. Your task is to conduct exploratory data analysis (EDA) to identify patterns in the data, ensuring that applicants who are capable of repaying their loans are not unfairly rejected.

##### **Dataset**:
> The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following nine diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

Following is the count of images present for each class of disease in decreasing order:

![image](https://github.com/user-attachments/assets/0d48ce12-c1f1-4688-a937-0aa04a8ddaa9)





## Libraries Used

- Python
- Pandas
- NumpPy
- Tensorflow
- Keras
- Matplotlib
- Seaborn
- Scikit
- Glob
- Pathlib
- OS
- Augmentor

## Steps Involved

- Mounting the data on Google Drive and loading the data inside the Python notebook
- Checking the count of images available in "Train" and "Test" dataset
- Forming the Train and Test datasets
- Visualizing the data
- Creating, Compiling, Training and Visualizing CNN Model 1
- Applying data augmentation on the Training dataset
- Creating, Compiling, Training and Visualizing CNN Model 2 (With Data Augmentation & Dropout Layer)
- Checking Class Distribution of our Training Dataset
- To address this class imbalance, we used the Augmentor library to generate new samples artificially
- Visualizing the distribution of augmented data after adding new images to the Training dataset
- Creating, Compiling, Training and Visualizing CNN Model 3 (With New Data from Augmentor)
- Creating, Compiling, Training and Visualizing CNN Model 4 (With L2 Regularization and Additional Dropout Layers)
- Checking the Test accuracy using Model 4 (With L2 Regularization and Additional Dropout Layers) using Test dataset
- Writing Conclusions




## Conclusions

> After 30 Epochs, using CNN Model 4 (With L2 Regularization and Additional Dropout Layers), the training accuracy is 87% and validation accuracy is 82%. As the difference between them is withing a range of 5%, the Model 4 seems to be optimum.
