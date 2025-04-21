#  Deploying a Mask R-CNN Image Segmentation Model on GCP with uWSGI & Flask

## Overview

This project demonstrates how to take a Mask R-CNN model for image segmentation from development to deployment using MLOps best practices on the Google Cloud Platform (GCP). The solution walks through building a **web application using Flask** and deploying it on GCP using **uWSGI**, **Docker**, **Cloud Build**, **Cloud Functions**, and **Kubernetes**. It’s a full-stack ML project that integrates deep learning, scalable architecture, and CI/CD automation.

## Dataset

This project assumes the Mask R-CNN model has already been trained on an image segmentation dataset like **MS COCO**. While the focus is on MLOps deployment, the model can be fine-tuned beforehand on any object detection and segmentation dataset suitable for your use case.

- **Dataset Example**: MS COCO (Common Objects in Context)
- **Data Type**: Image + Segmentation Masks
- **Target**: Multiple object classes with pixel-wise annotations
- **Attributes**: Class labels, bounding boxes, masks

## Tech Stack

| Category        | Tools/Technologies                                 |
|----------------|-----------------------------------------------------|
| Programming     | Python                                              |
| Deep Learning   | TensorFlow, `mrcnn`                                 |
| Backend         | Flask, uWSGI                                        |
| Containerization| Docker                                              |
| Deployment      | Google Cloud Platform (GCP), Kubernetes             |
| CI/CD           | Cloud Build, Cloud Source Repositories, Pub/Sub     |
| Monitoring      | GCP Cloud Logging, Cloud Functions                  |

## Project Workflow

### 1. **Project Setup**
- Clone/create a repository using **Cloud Source Repositories**.
- Understand folder structure for cloud-triggered deployment.

### 2. **Model Preparation**
- Use a pre-trained **Mask R-CNN** model built with TensorFlow.
- Save model files for inference (`.h5`, `.pkl`, or saved model format).

### 3. **Flask Application with uWSGI**
- Create a Flask API to accept image uploads and return segmented results.
- Configure `uWSGI` to serve the Flask app with a `.ini` configuration file.

### 4. **Dockerization**
- Write a `Dockerfile` to containerize the Flask + uWSGI app.
- Use **Google Cloud Build** to build the Docker image automatically.

### 5. **Kubernetes Deployment**
- Write necessary Kubernetes YAML configs (`deployment.yaml`, `service.yaml`).
- Deploy using GKE (Google Kubernetes Engine) to serve the model at scale.

### 6. **CI/CD Pipeline with GCP**
- Use **Cloud Build Triggers** to automate deployment on code commit.
- Configure **Pub/Sub** to trigger **Cloud Functions** (e.g., image processing events).

### 7. **Model Serving & Inference**
- Send image files to the Flask endpoint.
- Visualize results with overlaid masks and object labels.

## Expected Outcomes

- A fully functional image segmentation web app deployed on GCP.
- Automated CI/CD pipeline triggered on repository updates.
- Real-time serving of Mask R-CNN predictions via Flask API.
- Scalable and production-grade MLOps setup using Google Cloud services.


## Learning Takeaways

By the end of this project, you’ll have learned:

- How to operationalize deep learning models using **MLOps best practices**
- Integration of **Flask, uWSGI, and Docker** for efficient model serving
- Automating deployment using **GCP Cloud Build**, **Source Repositories**, and **Pub/Sub**
- End-to-end deployment pipeline using **Kubernetes** and **Cloud Functions**
- How to manage large-scale, reliable ML systems in production

## Hands-On Solution Code

[MLOps Project to Deploy an Image Segmentation Model on GCP](https://www.projectpro.io/project-use-case/mlops-project-deploy-mask-rcnn-model-using-flask-tensorflow)
