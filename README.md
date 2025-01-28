# Defect_Detection
This repository contains a project focused on defect detection using the DAGM dataset. The goal of this project is to classify and localize defects in industrial images using various deep learning models, including VGG16, ResNet, AlexNet, and a hybrid model combining ResNet and DenseNet.

## Overview

Defect detection is a crucial task in industrial automation to ensure product quality. This project utilizes the DAGM dataset, which includes images of industrial surfaces with and without defects. By leveraging deep learning models, we aim to detect defects with high accuracy while exploring the performance of individual and hybrid architectures.

## Dataset

The DAGM dataset provides:

- Training Images: Annotated images with labeled defects.
- Test Images: Images for evaluating the model's performance.

## Models Used

- VGG16: Fine-tuned for defect detection
- ResNet: Residual learning framework
- AlexNet: Simplified CNN architecture
- Hybrid Model: Combines ResNet and DenseNet for feature extraction. Provides a balance between accuracy and computational efficiency.

## Methodology

### Preprocessing:
- Images were resized to 224x224 to match the input dimensions of the models.
- Applied normalization to scale pixel values between 0 and 1.
- Augmented data with techniques like rotation, flipping, and zoom to increase diversity and prevent overfitting

### K-Fold Cross-Validation:
- Implemented 5-fold cross-validation to ensure robustness and generalizability of model performance.
- Each fold was used as a test set while the remaining were used for training, ensuring unbiased evaluation.

### Model Training
- Used Adam optimizer with a learning rate of 0.001.
- Binary Cross-Entropy (BCE) was employed as the loss function for binary classification.

### Evaluation Metrics:
- Accuracy
- Precision, Recall, and F1-Score

## Results
![image](https://github.com/user-attachments/assets/e5ec1e31-623c-478c-81a9-ac8b31e7e8b8)





