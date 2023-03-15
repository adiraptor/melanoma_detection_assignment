# Melanoma Cancer Detection
> Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
This project uses convolutional neural networks to try to accurately predict malignant melanoma pigments amongst a dataset of images consisting of malignat nad non malignant skin diseases. the dataset consists of 2239 training images and 118 test images.


## Conclusions
- Upon initial analysis of the dataset, the size of the dataset was very small, and, as predicted it lead to overfitting of the model.
- Without regularization and dropouts, training accuracy for the model was around 90% whereas validation accuracy was 43%
- I attempted to solve this using initial augmentation by flipping images and adding dropout layers, which bumped up the validation accuracy to around 50%, but still did not solve the problem of overfitting.
- Upon further analyzing the dataset, it was found that the classes were severely imbalanced - with melanoma being one of the most highly populated classes
- Upon introducing class rebalance, this problem was resolved entirely and led to a vlaidation accuracy of 82%.



## Technologies Used
- tensorflow==2.11.0
- Pillow==8.4.0
- Augmentor==0.2.10
- matplotlib==3.5.3
- numpy==1.22.4
- pandas==1.4.4

## Contact
Created by [@adiraptor] - feel free to contact me!

<!-- ## License -->
<!-- This project is open source and available under the [Apache 2.0 License](). -->