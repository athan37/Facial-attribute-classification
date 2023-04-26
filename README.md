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

Test loss: 0.4835874140262604

Test accuracy: 0.5479999780654907


**Transfer learning with EfficientNet:**

Test loss: 0.6156396269798279

Test accuracy: 0.7400000095367432

## Evaluation

We initially attempted to train and predict 50 facial attributes using binary_crossentropy, but the results were unsatisfactory as it was difficult to accurately predict all 50 traits for each individual. As a result, we chose to focus on separate trait pairs. Our first attempt with a basic CNN model yielded a 54% accuracy, while employing EfficientNet increased the accuracy to 74%.


