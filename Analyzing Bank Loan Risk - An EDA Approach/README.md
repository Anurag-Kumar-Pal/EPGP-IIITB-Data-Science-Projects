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
