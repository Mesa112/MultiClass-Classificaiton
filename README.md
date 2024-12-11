# Multi-Label Object Detection using YOLOv8

This project focuses on multi-label object detection using the YOLOv8 model. The objective is to detect and classify objects from five selected classes in the PASCAL VOC dataset. The model was trained to achieve high accuracy in both object detection and classification tasks.

## Features

- **Multi-label classification**: Detects the presence or absence of objects in a single image for five selected classes.
- **YOLOv8 Integration**: Utilizes the YOLOv8 architecture for efficient and real-time object detection.
- **Dataset Preprocessing**: Includes tools for converting PASCAL VOC annotations to YOLO format.
- **Performance Evaluation**: Provides metrics like mAP@50, precision, recall, and F1 score.

## Project Structure

```
├── dataset/                    # Organized training and validation datasets
│   ├── train/                 # Training images and labels
│   └── val/                   # Validation images and labels
├── scripts/                   # Scripts for dataset preprocessing, training, and evaluation
│   ├── preprocess.py         # Converts VOC annotations to YOLO format
│   ├── train.py             # Script for training the YOLOv8 model
│   └── evaluate.py          # Evaluates model performance
├── models/                   # Pretrained YOLOv8 models
│   └── yolov8n.pt          # YOLOv8n model weights
├── results/                 # Output results (metrics, graphs, predictions)
│   ├── metrics.png         # Training and validation metrics over epochs
│   ├── confusion_matrix.png
│   └── precision_recall.png
├── README.md               # Project documentation
└── dataset.yaml           # YOLO dataset configuration file
```

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.8+
- `pip` package manager
- `virtualenv` (optional but recommended)

### Setup

1. **Clone the repository**:
   ```bash
   git clone git@github.com:Mesa112/your-repo.git
   cd your-repo
   ```
