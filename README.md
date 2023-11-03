# Melanoma Detection Assignment
> To build a multiclass classification model using a custom convolutional neural network in TensorFlow. 


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- What is the background of your project?

    * Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


- What is the dataset that is being used?

    * The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


    * The data set contains the following 9 diseases:

        * Actinic keratosis
        * Basal cell carcinoma
        * Dermatofibroma
        * Melanoma
        * Nevus
        * Pigmented benign keratosis
        * Seborrheic keratosis
        * Squamous cell carcinoma
        * Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
1. In the 1st attempt to create CNN model to accurately detect 9 classes present in the dataset with 20 epochs in training phase.
    * The model was underfitting the data. Both training and validation accuracies were low, and both losses were high.

    * The model might not have enough capacity to learn from the data, or features it is learning are not informative enough.

2. In the 2nd attempt to create CNN model with data augmentation strategy to accurately detect 9 classes present in the dataset with 20 epochs in training phase.
    * The class "actinic keratosis" has the least number of samples.

    * The classes "pigmented benign keratosis" and "nevus" dominate the data in terms of proportionate number of samples, with "pigmented benign keratosis" having the highest number.

3. In the 3rd attempt to create CNN model by rectifying class imbalances (Augmentor library) to accurately detect 9 classes present in the dataset with 30 epochs in training phase.
    * The model's performance on the training data is very good with an accuracy of 96.46%.¶

    * The validation accuracy of 84.19% indicates that the model is also performing well on unseen data, although there's a gap between training and validation accuracy (~12%).

    * Overfitting: There are few signs of overfitting since the training accuracy keeps rising, but the validation accuracy varies.

    * Underfitting: The model doesn't show signs of underfitting since the training accuracy and loss are moving in the expected directions (accuracy increasing and loss decreasing).

    * The class rebalance helped reduce the overfititng of the data.

    * Employing more data augmentation, dropout, or regularization may further reduce the overfitting.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- pathlib - Version 1.0.1
- tensorflow - Version 2.10.0
- keras - Version 2.10.0
- matplotlib - Version 3.7.0
- numpy - Version 1.23.5
- pandas - Version 1.5.3


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Liverpool John Moores University & IIIT Bangalore
AI/ML MSc. Degree assignment on Melanoma Detection Assignment.


## Contact
Assignment done by Karthik Jayaraman [@karthikjram] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->