# Melanoma Skin Cancer Detection

## Abstract
In cancer, there are over 200 different forms. Out of 200, melanoma is the deadliest form of skin cancer. The diagnostic procedure for melanoma starts with clinical screening, followed by dermoscopic analysis and histopathological examination. Melanoma skin cancer is highly curable if it gets identified at the early stages. The first step of Melanoma skin cancer diagnosis is to conduct a visual examination of the skin's affected area. Dermatologists take the dermatoscopic images of the skin lesions by the high-speed camera, which have an accuracy of 65-80% in the melanoma diagnosis without any additional technical support. With further visual examination by cancer treatment specialists and dermatoscopic images, the overall prediction rate of melanoma diagnosis raised to 75-84% accuracy. The project aims to build an automated classification system based on image processing techniques to classify skin cancer using skin lesions images.

## Problem Statement
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
The data set contains the following diseases:

1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion
 

NOTE: You don't have to use any pre-trained model using Transfer learning. All the model building process should be based on a custom model.


## Motivation
To create a multiclass classification model using a custom convolutional neural network in tensorflow.

## Dataset
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). 
All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

The data set contains the following diseases:

![diseases](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/Diseases.png)

### Sample images from Dataset

![sample images](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/Sample_Images_Used.png)

## CNN Architecture Design
To classify skin cancer using skin lesions images. To achieve higher accuracy and results on the classification task, I have built custom CNN models.


### Model Architecture 1
![ModelArch1](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/ModelArchitecture1.png)

### Model Evaluation 1
![ModelEvaluation1](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/AccuracyVsLoss_2.png)

### Model Architecture Final
![ModelArch2](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/ModelArchitecture2.png)

### Model Evaluation Final
![ModelEvaluation2](https://github.com/prixroxx/Melanoma-Detection-CNN/blob/main/Melanoma_ReadMe_Resources/AccuracyVsLoss_2.png)

## Conclusion
The class rebalance helped in reducing overfitting of the data and thus the loss is being reduced. But it reduced the accuracy a little.

- Initially we tried without the ImageDataGenerator which created data to overfit at high ratio.
- Then we introduced dropout and ImageDataGenerator which reduced the overfitting.
- At last we tried Batch Normalization and Augumentation which really helped in carry forward.

## References
Melanoma Skin Cancer from https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html

Introduction to CNN from https://www.geeksforgeeks.org/introduction-convolution-neural-network/
