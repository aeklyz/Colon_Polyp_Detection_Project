# Deep Learning-Based Detection of Colonic Polyps in Pediatric Colonoscopy

## Overview
This project presents a deep learning-based system for detecting and segmenting colonic polyps in pediatric colonoscopy images. It applies instance segmentation to achieve precise localization at the pixel level.

## Dataset
The dataset used in this study consists of annotated pediatric colonoscopy images. 
Due to privacy and research constraints, the annotated dataset is not publicly available.

For demonstration purposes, sample images or publicly available datasets may be used.

## Features
- Instance segmentation for accurate polyp detection
- Data augmentation for improved generalization
- Real-time inference capability
- Optional web-based deployment using Gradio

## Methodology
- Model: YOLO-based instance segmentation architecture
- Dataset: Annotated pediatric colonoscopy dataset
- Preprocessing:
  - Image resizing to 640x640
  - Data augmentation (rotation, flipping, brightness adjustment, noise injection)
- Deployment: Optional web interface for real-time prediction

## Results
- Box mAP@0.50: 0.966
- Mask mAP@0.50: 0.974
- F1 Score: Approximately 0.96
- High precision and recall across test data

## Tech Stack
- Python
- PyTorch
- Ultralytics YOLO
- OpenCV
- Gradio

## How to Run
```bash
pip install -r requirements.txt
python app.py
