# Facial Attribute Classification
## Duc Anh Than and Sammy Sasaki

## Abstract

Facial attribute classification is the task of predicting attributes or characteristics of a person's face, such as gender, age, or facial expression. This repository provides an implementation of a facial attribute classification system using deep learning techniques.

Our system is based on a Convolutional Neural Network (CNN) architecture, which takes an input image and outputs a set of attribute predictions. The CNN is trained on a large-scale dataset of labeled facial images, and we use transfer learning to fine-tune the pre-trained network for our specific task.

We evaluate the performance of our system on a test set of facial images, and report accuracy and other relevant metrics. We also provide scripts to visualize the predictions of our system on new facial images.

## Model

Basic CNN model:
Test loss: 0.4835874140262604
Test accuracy: 0.5479999780654907

Transfer learning with EfficientNet:
Test loss: 0.6156396269798279
Test accuracy: 0.7400000095367432

## Evaluation

We first tried training and predicting 50 traits for the facial attributes with 'binary_crossentropy', however, it doesn't produce good result because it's hard to predict all 50 traits correctly for each person. Because of that, we decided to break down into different pair of traits. We first train on the basic CNN model and got the accuracy of 54%. Next, we tried with EfficientNet and the accuracy improves to 74%.

##How to load and run the code

1. Add data file to the root path of your drive: https://drive.google.com/file/d/1Sxt3FXYSymy-dbVhOGg99P7tJOyKGQUY/view?usp=sharing
2. Add label file to the root path of your drive: https://drive.google.com/file/d/0B7EVK8r0v71pblRyaVFSWGxPY0U/view?usp=sharing&resourcekey=0-YW2qIuRcWHy_1C2VaRGL3Q
3. Run the first line of the Colab and connect it to your drive
4. Rull the rest of the Colab
