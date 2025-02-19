# Melanoma Detection
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis..


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- a multiclass classification model using a custom convolutional neural network in TensorFlow. 
- Cancer detection model
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- We could draw below conclusions - rmsprop and adam optimizers gave similar results (overfitting the model) - however with sgd model remained underfit - For this experimentation I am going with rmsprop optimizer - As we can see that both training and validations accuracy are apart from each other, while training accuracy touching 90%, validation accuracy is fluctuating between 20-30% this shows that model is kind of overfit

| Configuration                 | Observations |
|--------------------------------|-------------|
| Simple Model                  | Even simple model with augmenter performed much better than without augmenter. That means the more data we have, the better the model. |
| With one extra layer          | Added one extra layer as validation accuracy kept fluctuating. |
| With Dropout                  | Added one dropout layer with 0.2 and found that validation accuracy was a bit stabilized. |
| Added more layers and dropouts | Training of the network became much more stable; accuracy and validation accuracy followed tightly together, so decided to increase the epochs and observe. |
| With Callback                 | Added two callbacks for saving the model and early stopping. The model stopped on a specific epoch with validation accuracy. |
| 70 Epochs                     | Found that with 70 epochs, accuracy and validation accuracy settled around 85% and 87%, respectively. The model looked fairly stable, so stopped training. |



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- TensorFlow Version: 2.18.0
- Keras Version: 3.8.0
- Augmentor Version: 0.2.12
- Matplotlib Version: 3.10.0
- NumPy Version: 1.26.4
- Pandas Version: 2.2.2
- Pillow Version: 11.1.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [@aakashbhardwaj27] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->