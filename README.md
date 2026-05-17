# Part 2: Computer Vision Problem Formulation and CNN Prototype

## Overview
This project builds a CNN model to classify manufacturing defect images into 4 categories.

---

# Dataset
- Source: Synthetic Manufacturing Defect Image Dataset
- Classes: normal, scratch, dent, stain
- Total Images: 480 (120 per class)
- Image Size: 128×128×3
- Train/Test Split: 80/20

---

# Task 1: Problem Identification

## Problem Type: Image Classification

## Why This Problem Type?
- Each image belongs to one defect category
- The goal is to predict the correct class of the image
- The project does not detect object locations
- The project does not perform pixel-level segmentation
- Therefore, image classification is the correct computer vision problem type

---

# Task 2: Dataset Exploration

- Number of classes: 4
- Classes: normal, scratch, dent, stain
- Images per class: 120
- Total images: 480
- Images resized to: 128×128
- Dataset is balanced because all classes have equal number of images

---

# Task 3: Image Preprocessing

The following preprocessing steps were applied:

- Resized all images to 128×128
- Normalized pixel values to range 0-1
- Split dataset into training and testing sets
- Applied data augmentation in Model 3

---

# Task 4: CNN Model Creation

The CNN models were created using TensorFlow and Keras.

## Layers Used
- Convolution Layer
- ReLU Activation Function
- Max Pooling Layer
- Flatten Layer
- Dense Layer
- Softmax Output Layer

---

# Task 5: Model Training and Evaluation

Four CNN models were trained and compared.

## Evaluation Methods
- Training Accuracy
- Testing Accuracy
- Training Loss
- Testing Loss
- Confusion Matrix
- Sample Predictions

## Best Model
Model 1 performed well on both training and testing data with high accuracy.

---

# Task 6: CNN Concept Explanation

## What is Convolution?
Convolution is a process where filters move across the image to detect important features such as edges, textures, and patterns.

## Why is Pooling Used?
Pooling reduces the image size while keeping important information. This helps reduce computation and prevents overfitting.

## Why is ReLU Commonly Used?
ReLU helps the model learn complex patterns by introducing non-linearity. It also makes training faster.

## Why are CNNs Better Than Feed-Forward Networks?
CNNs are better for images because they can automatically learn visual patterns and spatial relationships using fewer parameters.

---

# Task 7: Business Use Case Mapping

## Manufacturing Quality Inspection

This type of computer vision system can be used in manufacturing industries for automatic defect detection.

### Example
- Normal products can be approved
- Scratched products can be reworked
- Dented products can be rejected
- Stained products can be identified quickly

## Benefits
- Faster inspection
- Reduced human error
- Better product quality
- Lower inspection cost

---

# Files Included

- notebook.ipynb
- README.md
- requirements.txt
- accuracy_loss_curves.png
- confusion_matrix.png
- prediction_outputs.png
- best_cnn_model.h5

---

# How to Run the Project

1. Install required libraries

```bash
pip install tensorflow pillow pandas numpy scikit-learn matplotlib seaborn jupyter