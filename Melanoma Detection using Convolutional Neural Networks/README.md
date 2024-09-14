![image](https://github.com/heyitsanuragpal/MelanomaDetectionCaseStudy/assets/151669975/0b49713d-1b53-4600-b746-512089af0c95)# Detection of Melanoma Skin Cancer using CNN
> Developing a custom convolutional neural network in TensorFlow for a multiclass classification model for detecting Melanoma skin cancer.

## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Steps Involved](#steps-involved)
* [Conclusions](#conclusions)


## General Information

> **Problem Statement**:
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

> **Dataset**:
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

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

![image](https://github.com/heyitsanuragpal/Melanoma-Detection/assets/151669975/8170fb29-5c7a-4873-931d-d2368440e1a9)



## Technologies Used

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
