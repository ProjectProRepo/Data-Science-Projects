# Face Recognition System in Python using FaceNet

## Overview
This deep learning project demonstrates how to build a **Face Recognition System** in Python using **FaceNet** and **OpenCV**. By leveraging powerful pre-trained models like FaceNet and VGGFace, along with Haar Cascade classifiers for face detection, the system can accurately identify individuals from images and videos. The solution includes face extraction, embedding generation, visualization using t-SNE, and face classification using a machine learning model.

### Key Objectives:
- Detect and extract faces from videos and images.
- Generate facial embeddings using FaceNet.
- Train a classifier (SVM) on these embeddings.
- Recognize and label individuals in new images and videos.

---

## Dataset

- **Source:** Extracted from the popular sitcom *Friends* video on [YouTube](https://www.youtube.com/watch?v=NzOTuh63eVs).
- **Training Data:** 35 images (7 per person for 5 characters: Rachel, Chandler, Phoebe, Monica, Ross).
- **Test Data:** 15 images across the same characters.
- **Data Format:** JPG images extracted from video frames.
- **Annotation:** Faces are detected using Haar Cascade and manually verified.

---

## Tech Stack

### Language
- Python (3.6.2)

### Libraries & Tools
- **Computer Vision:** OpenCV, skimage, imutils
- **Deep Learning:** TensorFlow, Keras, FaceNet, VGGFace
- **Machine Learning:** scikit-learn (SVM for classification)
- **Visualization:** matplotlib, t-SNE
- **Utilities:** os, numpy, pytube (for video downloading)

---

## Project Workflow

### 1. Video Processing
- Download video from YouTube.
- Extract frames per second from the video.

### 2. Face Detection & Extraction
- Use **Haar Cascade Classifier** to locate faces in each frame.
- Resize and preprocess faces as required by the FaceNet model.

### 3. Embedding Generation
- Extract 128-dimensional facial embeddings using the **pre-trained FaceNet model**.
- Normalize embeddings before training.

### 4. Classification
- Train an **SVM model** on the facial embeddings.
- Use trained model to classify new/test images.

### 5. Inference & Labeling
- Detect faces in test frames or video using Haar Cascade.
- Generate embeddings and predict labels using the trained SVM model.
- Overlay names on recognized faces in frames.

### 6. Visualization
- Use **t-SNE** to visualize high-dimensional embeddings.
- Plot example predictions on test images and videos.

---

## Expected Outcomes

By the end of this project, you will have:
- A complete face recognition system capable of identifying people from images or video.
- A trained classifier using facial embeddings.
- Visualization of facial feature space using dimensionality reduction.

---

## Learning Takeaways

- Understand **Face Recognition** pipeline using real-world video data.
- Learn to work with **FaceNet embeddings** and **VGGFace architecture**.
- Gain experience with **Haar Cascade classifiers** for object detection.
- Build an end-to-end system integrating **OpenCV**, **deep learning models**, and **machine learning classifiers**.
- Apply **t-SNE** to visualize high-dimensional data in 2D.

---

## Hands-On Solution Code
[
Face Recognition Project with Source Code](https://www.projectpro.io/project-use-case/face-recognition-python-project)
