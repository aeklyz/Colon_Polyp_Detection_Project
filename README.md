# Deep Learning-Based Detection of Colonic Polyps in Pediatric Colonoscopy

## Overview
This project presents a deep learning-based system for detecting and segmenting colonic polyps in pediatric colonoscopy images. It applies instance segmentation to achieve precise localization at the pixel level.

## Dataset
The dataset used in this project consists of pediatric colonoscopy images sourced from a publicly available dataset:

https://academictorrents.com/details/d8653db45e7f111dc2c1b595bdac7ccf695efcfd

The dataset was manually annotated as part of this research to support supervised learning for polyp detection and segmentation.

Due to research and data-sharing restrictions, the annotated dataset is not publicly available.

Users may access the original unannotated dataset using the link above and apply their own annotation pipeline if needed.

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

1. Install dependencies:
pip install -r requirements.txt

2. Run inference:
python src/predict.py
