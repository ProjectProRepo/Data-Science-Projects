# Forecasting Business KPIs with TensorFlow and Python

## Overview

This machine learning project demonstrates how to forecast **key performance indicators (KPIs)** related to brand visibility in sports broadcasts, using **video data and object detection models**. By analyzing an IPL cricket match video clip, the goal is to identify the **appearance frequency**, **frame position**, and **area coverage** of brand logos using a deep learning pipeline powered by **TensorFlow Object Detection API**.

The solution encompasses end-to-end processing: from video extraction, frame annotation, and model training to KPI metric computation based on logo occurrences.

---

## Business Objective

Brand visibility is a critical component of marketing ROI in televised sports. This project simulates a real-world branding analysis scenario by:
- Measuring **brand logo frequency**, 
- Identifying the **frames** where logos appear, and 
- Calculating the **smallest and largest area percentage** of logos during a sports event.

These insights can support **data-driven sponsorship valuation**, **brand impact studies**, and **ad placement optimizations**.

---

## Dataset

- **Source:** 2-minute 35-second clip from an IPL match between **CSK** and **RCB**, downloaded from YouTube.
- **Format:** 
  - Annotated using `LabelImg` into XML files.
  - Converted to CSV and TFRecord formats for training/testing.
- **Target Labels:** Brand logos appearing in the video frames.
- **Data Volume:**
  - Hundreds of annotated frames extracted from the match clip.

---

## Tech Stack

### Language
- **Python 3.x**

### Libraries & Tools
- **TensorFlow Object Detection API**
- **OpenCV** – for frame processing
- **Pillow (PIL)** – for image handling
- **Matplotlib** – for visualization
- **NumPy** – for numerical operations
- **uuid** – for unique filename generation
- **LabelImg** – for image annotation
- **TensorBoard** – for training monitoring

---

## Project Workflow

### Data Preparation
1. **Download video** using `youtube_downloader.py`.
2. **Extract frames** from video for annotation.
3. **Annotate images** using `LabelImg` → generate XML files.
4. **Convert XML → CSV** and then **CSV → TFRecord** (train/test).

### Model Setup & Training
5. **Clone TensorFlow Models** repository and setup Object Detection API.
6. **Download base model** (e.g., `ssd_resnet50_fpn_coco`) from TensorFlow Model Zoo.
7. **Update `pipeline.config`** for training parameters.
8. **Train model** using `train.py`.
9. **Monitor training** using TensorBoard (`events.out.tfevents.*`).

### Model Freezing & Export
10. Generate `frozen_inference_graph.pb` from `ckpt` files using `export_inference_graph.py`.

### Inference & KPI Extraction
11. **Make predictions** using `predict.py`.
12. **Modify `visualization_utils.py`** to extract class and score info.
13. **Break video into frames** and analyze each frame for detections.
14. **Run `video_processing.ipynb`** to compute:
    - Total appearances per logo
    - Shortest and longest logo area percentages
    - Frame-wise logo occurrences

---

## Expected Outcomes

- A trained object detection model capable of recognizing brand logos.
- Visual analysis of detections overlaid on video frames.
- Accurate computation of KPI metrics for each brand logo.
- End-to-end pipeline for video data annotation, training, and analysis.

---

## Learning Takeaways

By working on this project, you'll gain hands-on experience with:
- TensorFlow Object Detection API
- Model cloning and fine-tuning using transfer learning
- Data annotation and preprocessing for video-based deep learning
- Model exporting and inference using frozen graphs
- KPI metric generation from raw video data
- Visualization and debugging with TensorBoard

---

## Hands-On Solution Code
[**Forecasting Business KPIs with Tensorflow** ](https://www.projectpro.io/project-use-case/business-kpis-forecasting-with-python)
