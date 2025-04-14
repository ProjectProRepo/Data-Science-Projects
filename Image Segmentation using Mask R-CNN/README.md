# Image Segmentation using Mask R-CNN with TensorFlow

## Overview
This project focuses on using the Mask R-CNN deep learning model for early fire detection through image segmentation. The goal is to accurately identify and localize fire regions in images to help authorities take proper safety measures. Using TensorFlow, this project trains a Mask R-CNN model to detect fire in images by segmenting the fire pixels and predicting bounding boxes around the fire area.

### Key Objectives:
- Understand the concepts of image detection, localization, and segmentation.
- Learn how to implement a Mask R-CNN model for early fire detection.
- Understand the role of Region Proposal Network (RPN), ROI Classifier, and **bounding box regressors**.
- Perform **image annotation** and create the dataset for training the model.
- Build, train, and evaluate a deep learning model using **transfer learning** techniques.

## Dataset
The dataset consists of fire-related images in various formats (JPG, PNG, TIF), with a corresponding **annotation file** (`via_project.json`) that marks the regions of interest (fire areas).

### Dataset Details:
- **Training Data:** 20 images
- **Validation Data:** 10 images
- **Test Data:** 1 image
- **Annotation File:** Contains the region of interest (ROI) marked as fire pixels.

## Tech Stack
- **Programming Language:** Python
- **Libraries:**
  - `numpy`
  - `keras`
  - `tensorflow`
  - `mrcnn` (Mask R-CNN implementation)
  - `scikit-image`
  - `matplotlib`
- **Other Tools:**
  - **VGG Annotator** for manual annotation (Link: [VGG Annotator](https://www.robots.ox.ac.uk/~vgg/software/via/via_demo.html))

## Project Workflow

### 1. **Dataset Preparation:**
   - Use **VGG Annotator** to create annotations marking fire pixels in images.
   - Save annotations as JSON files containing the region of interest.

### 2. **Environment Setup:**
   - Install dependencies using the provided `requirements.txt` file.

### 3. **Image Loading and Preprocessing:**
   - Create classes to load and preprocess images and annotations for training and inference.
   - Load training and validation datasets along with the associated annotations.

### 4. **Model Configuration:**
   - Define configuration classes for training, including setting up backbone configurations for feature extraction.
   - Use pre-trained weights (e.g., **ResNet101**) for transfer learning.

### 5. **Model Building (Mask R-CNN):**
   - Build the Mask R-CNN model architecture for object detection and segmentation.
   - Train the model using the training data and validate it on the validation dataset.
   
### 6. **Training the Model:**
   - Train the model on fire detection images, utilizing annotated fire regions.
   - Store log files for each epoch to track the training progress.

### 7. **Inference and Evaluation:**
   - Make predictions on test images.
   - Visualize predictions by overlaying predicted masks and bounding boxes on test images.

### 8. **Results Visualization:**
   - Use `matplotlib` to visualize the segmentation results (bounding boxes and masks) over test images.

## Expected Outcomes
- A trained **Mask R-CNN** model capable of accurately detecting fire in images.
- Bounding boxes and masks generated around the fire regions.
- Insights into implementing image segmentation for real-world applications, such as early fire detection.

## Learning Takeaways
- **Image Localization and Segmentation:** Learn how to detect and segment specific regions in images.
- **Mask R-CNN Model:** Gain hands-on experience implementing and training the Mask R-CNN model for object segmentation.
- **Transfer Learning:** Understand how to leverage pre-trained weights (e.g., ResNet101) to improve model performance.
- **Fire Detection:** Apply deep learning for real-world applications like early fire detection in images.

## Hands-On Solution Code
[Image Segmentation using Mask RCNN with Source Code
](https://www.projectpro.io/project-use-case/image-segmentation-mask-rcnn)
