# Project Name
> Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis. Task is to build a CNN model which can able to detect melanoma out of various skin cancers such as, 
1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
6. 5. Nevus
7. Pigmented benign keratosis
8. Seborrheic keratosis
9. Squamous cell carcinoma
10. Vascular lesion

# Project Pipeline

Data Reading/Data Understanding → Defining the path for train and test images 
Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
Dataset visualization → Create a code to visualize one instance of all the nine classes present in the dataset 


## Model Building & training : 

Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
Choose an appropriate optimizer and loss function for model training
Train the model for ~20 epochs
Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit.
Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 


## Model Building & training on the augmented data :

Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
Choose an appropriate optimizer and loss function for model training
Train the model for ~20 epochs
Write your findings after the model fit, see if the earlier issue is resolved or not?
Class distribution: Examine the current class distribution in the training dataset 
- Which class has the least number of samples?
- Which classes dominate the data in terms of the proportionate number of samples?
Handling class imbalances: Rectify class imbalances present in the training dataset with Augmenter library.


## Model Building & training on the rectified class imbalance data :

Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
Choose an appropriate optimizer and loss function for model training
Train the model for ~30 epochs
Write your findings after the model fit, see if the issues are resolved or not?


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Out of 9 skin cancers, task is to Classify various skin cancers appropriately
- Building a model using Convolutional neural networks 
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant. The data set contains the following diseases:

1. Actinic keratosis
2. Basal cell carcinoma
3, Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- First CNN model was built with 4 conv2D layers and one fully connected Dense layer
- Second CNN model built by applying some augmentation strategy to get rid of overfitting/underfitting occurred by first model and adding some Dropout layers.
- Third CNN model(train accuracy=91, validation accuracy=87) was built after applying augmentation(to overcome class imbalance in the training dataset)
- Finally choosing the best model out of three based on train and validation accuracies, Predict and evaluate Test images accuracy and loss.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- TensorFlow - version 2.17.0
- Keras - version 3.4.1
- Numpy - version 1.26.4

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project was inspired by UpGrad IIITBanglore

## Contact
Created by [@UmaHyndavi] - feel free to contact me!
## Nbviewer link
https://nbviewer.org/github/UmaHyndavi/Melanoma_Detection_Assignment/blob/master/Uma_Hyndavi_nn.ipynb


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->