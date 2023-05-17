# Facial Attribute Classification
## Duc Anh Than and Sammy Sasaki

## Abstract

Facial attribute classification is the task of predicting attributes or characteristics of a person's face, such as gender, age, or facial expression. This repository provides an implementation of a facial attribute classification system using deep learning techniques.

Our system is based on a Convolutional Neural Network (CNN) architecture, which takes an input image and outputs a set of attribute predictions. The CNN is trained on a large-scale dataset of labeled facial images, and we use transfer learning to fine-tune the pre-trained network for our specific task.

We evaluate the performance of our system on a test set of facial images, and report accuracy and other relevant metrics. We also provide scripts to visualize the predictions of our system on new facial images.

## How to load and run the code

1. Add data file to the root path of your drive: https://drive.google.com/file/d/1Sxt3FXYSymy-dbVhOGg99P7tJOyKGQUY/view?usp=sharing
2. Add label file to the root path of your drive: https://drive.google.com/file/d/0B7EVK8r0v71pblRyaVFSWGxPY0U/view?usp=sharing&resourcekey=0-YW2qIuRcWHy_1C2VaRGL3Q
3. Run the first line of the Colab and connect it to your drive
4. Rull the rest of the Colab

## Model

**Basic CNN model:**

Test loss: 0.502

Test accuracy: 0.762


**Transfer learning with MobileNetV2:**

Test loss: 0.468

Test accuracy: 0.762

## Evaluation

We initially attempted to train and predict 50 facial attributes using binary_crossentropy, but the results were unsatisfactory as it was difficult to accurately predict all 50 traits for each individual. As a result, we chose to focus on separate trait pairs. Our first attempt with a basic CNN model yielded a 0.762% accuracy, while employing MobileNetV2 generate similar results.


