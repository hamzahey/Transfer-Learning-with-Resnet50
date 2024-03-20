# Plant Disease Classification using ResNet50

This repository contains code for classifying plant diseases using the ResNet50 model with transfer learning. The dataset used for training and evaluation is the [New Plant Diseases Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset) available on Kaggle.

## Overview

The goal of this project is to classify different plant diseases using deep learning techniques. Specifically, we employ the ResNet50 architecture, which has shown promising results in image classification tasks.

## Dataset

The dataset consists of images of various plant diseases and healthy plant leaves. It includes multiple classes of diseases, each containing images of affected plants. The dataset is divided into training and testing sets.

## Methodology

1. **Model Selection**: ResNet50 is chosen as the base architecture for its effectiveness in image classification tasks and its availability in popular deep learning frameworks.

2. **Transfer Learning**: We utilize transfer learning by leveraging the pre-trained ResNet50 model. The final classification layer is replaced with a new fully connected layer to match the number of classes in the plant disease dataset.

3. **Training Strategy**: We experiment with two different training strategies:
   - Fine-tuning: In this approach, we fine-tune the pre-trained ResNet50 model on the plant disease dataset, allowing the model to adjust its parameters to better suit the task.
   - Feature Extraction: Here, we freeze the weights of the pre-trained ResNet50 model and only train the new fully connected layer. This serves as a feature extractor, where the pre-trained layers act as feature detectors.

## Results and Analysis

We evaluate the performance of the trained models on the test dataset and compare the results obtained from fine-tuning and feature extraction approaches. Additionally, we analyze the model's performance on different disease classes to identify areas for improvement and potential future research directions.

