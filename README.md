# Multi-Label Object Detection using YOLOv8

This project implements a multi-label object detection system using YOLOv8, trained on the PASCAL VOC dataset. The model successfully detects and classifies objects in real-time, demonstrating strong performance across multiple object classes.

## Detection Results

<table>
  <tr>
    <td align="center" width="33%">
      <img src="https://github.com/Mesa112/MultiClass-Classificaiton/raw/main/Multi_Class%20Classification/runs/detect/predict/WhatsApp%20Image%202024-12-09%20at%2014.15.26.jpg" width="100%">
      <br>
      <em>Street Detection Scene</em>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/Mesa112/MultiClass-Classificaiton/raw/main/Multi_Class%20Classification/runs/detect/predict/WhatsApp%20Image%202024-12-09%20at%2014.15.28.jpg" width="100%">
      <br>
      <em>Urban Environment Detection</em>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/Mesa112/MultiClass-Classificaiton/blob/main/Multi_Class%20Classification/runs/detect/predict/WhatsApp%20Image%202024-12-09%20at%2014.15.28%20(1).jpg" width="100%">
      <br>
      <em>Animal Detection</em>
    </td>
  </tr>
</table>

## Features

- **Real-time Detection**: Processes images and video streams with minimal latency
- **Multi-label Classification**: Detects multiple object classes simultaneously
- **High Accuracy**: Achieves 85% mAP@50 and 65% mAP@50-95
- **Robust Performance**: Handles varying lighting conditions and object scales
- **Efficient Processing**: Optimized for both CPU and GPU execution

## Model Architecture

The system uses YOLOv8 (You Only Look Once version 8) with the following specifications:
- Input Resolution: 640x640 pixels
- Backbone: CSPDarknet
- Training Epochs: 20
- Batch Size: 16
- Optimizer: SGD

## Dataset

The model was trained on the PASCAL VOC dataset with:
- 5,000+ annotated images
- Multiple object classes
- Varied environmental conditions
- Diverse object scales and orientations

## Project Structure

```
├── dataset/                    # Training and validation datasets
│   ├── train/                 # Training images and labels
│   └── val/                   # Validation images and labels
├── scripts/                   # Processing and evaluation scripts
│   ├── preprocess.py         # VOC to YOLO format converter
│   ├── train.py             # Model training script
│   └── evaluate.py          # Performance evaluation
├── models/                   # Model weights
│   └── yolov8n.pt          # YOLOv8 weights
├── results/                 # Performance metrics
│   ├── metrics.png         # Training metrics
│   ├── confusion_matrix.png
│   └── precision_recall.png
└── dataset.yaml            # Dataset configuration
```

## Performance Metrics

- **mAP@50**: 0.85
- **mAP@50-95**: 0.65
- **Precision**: Up to 90% for major classes
- **Inference Speed**: Real-time processing on GPU

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Contact

Esteban Mesa - [estebanmesa57@gmail.com](mailto:estebanmesa57@gmail.com)

Project Link: [https://github.com/Mesa112/MultiClass-Classificaiton](https://github.com/Mesa112/MultiClass-Classificaiton)
