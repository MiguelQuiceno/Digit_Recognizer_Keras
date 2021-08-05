# Digit_Recognizer_Keras(English)
This is a notebook from the "digit recognizer" competition in kaggle, in which i've got 99,53% Accuracy
<img src="https://user-images.githubusercontent.com/60410581/128421206-ade968bd-3ac6-4c2e-b7b2-36b17c413b1b.png" alt="image" width="500"/>

In this notebook i use a Convolutional Neural Network to predict the class of a given handwritten number:
## Model image:
![image](https://user-images.githubusercontent.com/60410581/128421557-aee4b5a4-1e46-4c3b-8fc8-0ab3aebd89a6.png)

## Description of Model:
* 2 Convolutional Blocks
    * Each block consists of 2 Conv2D layers with LeakyRelU activation layers. Then a MaxPool2D layer and finally a Dropout Layer.
* Then Dense Layers and Output layer after Flatten layer.
* MaxPool2D layer is used to reduce the size of the image. Pool size (2,2) means reducing the image from (28,28) to (14,14). Reducing the features.
* Dropout layer drops the few activation nodes while training, which acts as regularization. Do let the model to over-fit.
* Output layer has 10 nodes with sigmoid activation.

## Results:
With the help of image augmentation i was able to get very good results on the test set:

![image](https://user-images.githubusercontent.com/60410581/128421972-45940f38-0076-4c5e-b230-6f8a7a8c382f.png)

If you find this notebook useful, don't forget to give me a star on the github repo, and if its posible, on the kaggle notebook:
https://www.kaggle.com/miguelquiceno/digit-recognizer-keras?scriptVersionId=70307350
