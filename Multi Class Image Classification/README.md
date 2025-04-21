# Multi-Class Image Classification using CNN in Python

## Overview
This project demonstrates how to build a Sequential Convolutional Neural Network (CNN) model in Python to perform multi-class image classification. CNNs are inspired by how the human brain interprets visual input—by identifying patterns, shapes, and textures. In this hands-on implementation, we classify images into three distinct categories: Driving License, Social Security, and Others. This project provides a foundational understanding of CNNs and serves as a great entry point into computer vision with real-world relevance, such as autonomous driving and document classification.

---

## Dataset
The dataset used in this project contains categorized images for a multi-class classification task.

###  Key Details:
- **Classes**: Driving License, Social Security, Others
- **Training Set**: ~200 images per class
- **Testing Set**: ~50 images per class
- **Structure**: Each class is stored in a separate subfolder within the training and testing directories
- **Source**: (Assumed local or custom dataset – update with link if hosted)

The model learns to distinguish between document types by analyzing their visual features through multiple convolutional and pooling layers.


## Tech Stack

- **Language**: Python
- **Libraries**:
  - `numpy`: Numerical operations
  - `matplotlib`: Visualization
  - `cv2`: Image processing (OpenCV)
  - `tensorflow` / `keras`: Deep learning framework

## Project Workflow

### 1. **Library Imports**
Import essential packages for data manipulation, visualization, and model training.

### 2. **Data Loading & Visualization**
- Load images from folders using `ImageDataGenerator`
- Visualize sample images
- Plot class distribution using count plots

### 3. **Data Preprocessing**
- Normalize image pixel values
- Resize and reshape input data
- Create training and validation sets
- Augment data using transformations like rotation, zoom, and shift (to prevent overfitting)

### 4. **Model Building**
- Define a **Sequential CNN model**
- Add layers:
  - Convolutional layers for feature extraction
  - MaxPooling for dimensionality reduction
  - Dropout layers to prevent overfitting
Use **Softmax activation** in the final layer for multi-class prediction
- Compile the model with:
  - **Loss function**: `categorical_crossentropy`
  - **Optimizer**: `adam`
  - **Metrics**: `accuracy`

### 5. **Model Training**
- Train the model on the augmented dataset
- Monitor training and validation performance
- Adjust hyperparameters as needed

### 6. **Model Evaluation & Prediction**
- Predict on test data
- Generate confusion matrix and classification report
- Visualize predictions

### 7. **Save the Model**
- Export the trained model in `.h5` format for deployment or future use

## Expected Outcomes
- A working CNN model capable of classifying input images into one of three predefined categories
- Understanding how CNN layers work and interact
- Practical knowledge of model training, tuning, and saving
- Foundational exposure to computer vision tasks in Python

## Learning Takeaways

By completing this project, you'll gain hands-on experience with:

- Convolutional Neural Networks (CNNs)
- Concepts of convolution, pooling, and activation functions (ReLU, Softmax)
- Techniques for handling image data
- Multi-class classification in deep learning
- Data augmentation using `ImageDataGenerator`
- Saving and loading trained deep learning models

## Hands-On Solution Code

[Multi Class Image Classification Model Source Code](https://www.projectpro.io/project-use-case/multi-class-image-classification-python)
