# Build OCR from Scratch in Python using YOLO and Tesseract

## Overview

This project is a hands-on implementation of an **Optical Character Recognition (OCR)** system built from scratch using **YOLO v4 for object detection** and **Tesseract for text recognition**. The primary use case is to automate the extraction of crucial information from digital invoices—specifically the **Invoice Number**, **Billing Date**, and **Total Amount**. This end-to-end solution demonstrates how deep learning and OCR techniques can streamline manual business processes and reduce human labor.

## Dataset

A custom dataset of **invoice images** is used for training YOLO to recognize text regions.

- **Source**: Manually curated dataset of invoice images
- **Classes**: 
  - `invoice_number`
  - `billing_date`
  - `total_amount`
- **Annotations**: Labeled using [LabelImg](https://github.com/tzutalin/labelImg)
- **Format**: YOLO-compatible annotation files (`.txt` with bounding box coordinates)

## Tech Stack

| Category          | Tools/Technologies                                    |
|------------------|--------------------------------------------------------|
| Language          | Python                                                 |
| Object Detection  | YOLO v4 (via Darknet)                                  |
| OCR Engine        | Tesseract OCR                                          |
| IDE/Environment   | Google Colab                                           |
| Visualization     | OpenCV                                                 |
| Annotation Tool   | LabelImg                                               |
| Dependencies      | pytesseract, numpy, matplotlib, os, glob              |

## Project Workflow

### 1. **Set Up YOLO v4**
- Clone [AlexeyAB’s Darknet repo](https://github.com/AlexeyAB/darknet)
- Configure `Makefile` for OpenCV and GPU
- Build darknet with custom settings
- Download pre-trained YOLOv4 weights

### 2. **Data Collection & Annotation**
- Collect invoice images
- Annotate using **LabelImg** with custom classes
- Save annotations in YOLO format

### 3. **Prepare Training Configs**
- Customize `.cfg` file for YOLO
- Create `obj.data` and `obj.names`
- Split data into `train.txt` and `test.txt`

### 4. **Train Custom YOLO Model**
- Load pre-trained weights
- Fine-tune on invoice dataset
- Use transfer learning to improve training with fewer samples

### 5. **Evaluate Model**
- Use **Mean Average Precision (mAP)** to evaluate detection performance
- Visualize predictions using OpenCV

### 6. **Integrate Tesseract OCR**
- Use YOLO to detect regions of interest
- Apply Tesseract OCR on those regions to extract text
- Import and configure `pytesseract`
- Optionally fine-tune Tesseract’s LSTM model for better accuracy

### 7. **Post-Processing**
- Store and display detected classes with bounding boxes
- Save coordinates and recognized text separately

## Expected Outcomes

- A custom OCR pipeline capable of extracting key fields from invoice images
- Well-integrated use of **YOLO for detection** and **Tesseract for text extraction**
- Automated processing of invoices, reducing manual efforts
- A modular codebase that can be adapted to other OCR use cases

## Learning Takeaways

By completing this project, you’ll gain practical experience in:

- Object detection using YOLO v4
- OCR using Tesseract with LSTM
- Data labeling and annotation using LabelImg
- Working with OpenCV for image manipulation and visualization
- Model evaluation using mAP
- Google Colab for GPU-accelerated training
- Configuring deep learning workflows in Python

## Hands-On Solution Code

[Build OCR from Scratch Source Code
](https://www.projectpro.io/project-use-case/build-your-own-ocr-tesseract-yolo)

## Use Case

This OCR solution is ideal for businesses that process a large number of invoices manually. Automating invoice data extraction saves time, reduces errors, and improves operational efficiency across finance, procurement, and accounts departments.

