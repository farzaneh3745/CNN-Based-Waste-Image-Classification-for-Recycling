# CNN-Based Waste Image Classification for Recycling

## Project Overview

This project focuses on waste image classification using deep learning. The goal is to classify waste images into different categories and compare the performance of a Custom CNN model with transfer learning models.

CNN models are useful for this task because they can learn visual features from images, such as shape, color, texture, and edges.

## Dataset Information

The dataset used in this project is the **Garbage Classification (12 classes)** dataset from Kaggle.

Dataset link: https://www.kaggle.com/datasets/mostafaabla/garbage-classification

The dataset contains labeled waste images organized into 12 classes.

- Total images: 15,515
- Number of classes: 12
- Image type: RGB color images
- Target image size: 224 × 224
- Task type: Multi-class image classification

## Waste Classes

The dataset includes the following waste classes:

- battery
- biological
- brown-glass
- cardboard
- clothes
- green-glass
- metal
- paper
- plastic
- shoes
- trash
- white-glass

## Methodology

The main steps of the project are:

1. Load the dataset from Kaggle
2. Analyze the dataset and class distribution
3. Resize images to 224 × 224 pixels
4. Normalize image pixel values
5. Split the dataset into training, validation, and test sets
6. Apply data augmentation to the training images
7. Train a Custom CNN model
8. Train MobileNetV2 and ResNet50 using transfer learning
9. Evaluate all models
10. Save figures, tables, trained models, and comparison results

## Models Used

Three models were implemented and compared:

### Custom CNN

The Custom CNN was used as the baseline model. It was trained from scratch using convolutional layers, max pooling layers, global average pooling, dropout, and a softmax output layer.

### MobileNetV2

MobileNetV2 was used as a transfer learning model. The pre-trained base was frozen, and a new output layer was added for the 12 waste classes.

### ResNet50

ResNet50 was also used as a transfer learning model. It was used to compare a deeper pre-trained model with Custom CNN and MobileNetV2.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification reports
- Confusion matrices
- Accuracy and loss curves

Because the dataset is imbalanced, accuracy alone is not enough. Precision, recall, and F1-score were also used to evaluate model performance more carefully.

## Project Structure

```text
CNN-Based-Waste-Image-Classification-for-Recycling/
│
├── Notebook/
│   └── notebook-wasterecycling-codes.ipynb
│
├── Results/
│   ├── figures/
│   └── tables/
│
├── models/
│   ├── custom_cnn_best.keras
│   └── mobilenetv2_best.keras
│
└── README.md
