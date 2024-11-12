# Tumor Detection

This project uses a combination of state-of-the-art tools and libraries to train a YOLOv5 model for the task of tumor detection in MRI images. The project leverages Google Colab for execution, PyTorch for model development, and YOLOv5 for efficient object detection. It uses a structured workflow, including the installation of dependencies, model training, and result visualization, to develop a robust deep learning model for medical image analysis.

## YOLOv5

YOLOv5 (You Only Look Once version 5) is a real-time object detection model that’s widely used in computer vision applications for identifying and locating objects within an image or video. Developed by Ultralytics in 2020, YOLOv5 is part of the YOLO family of models, renowned for their balance of speed and accuracy, making them suitable for applications where real-time processing is crucial. While earlier versions of YOLO were developed in frameworks like Darknet, YOLOv5 is written entirely in PyTorch, making it more accessible, adaptable, and faster to deploy, especially for researchers and practitioners familiar with the PyTorch ecosystem. 
## Tools:
Python

Google Colab

YOLO v5

Pytorch

OpenCV

Matplotlib

## Model Training and Validation Performance
![Alt text](results.png)
The training and validation metrics over 50 epochs for the object detection model indicate effective learning and generalization. Key observations include:

### Losses (Top and Bottom Left Panels)
Training Losses: The train/box_loss, train/obj_loss, and train/cls_loss curves decrease consistently, indicating improvements in bounding box localization, objectness, and classification.
Validation Losses: The val/box_loss, val/obj_loss, and val/cls_loss curves show a similar downward trend as the training losses, suggesting that the model generalizes well with no signs of overfitting.

### Precision and Recall (Top Right Panels)
The metrics/precision and metrics/recall metrics exhibit an upward trend, stabilizing near 0.9 and 0.6, respectively. This demonstrates that the model’s accuracy in detecting objects improves and reaches a stable performance level over the epochs.

### Mean Average Precision (mAP) Scores (Bottom Right Panels)
The metrics/mAP_0.5 and metrics/mAP_0.5:0.95 scores increase steadily, reaching approximately 0.8 and 0.5, respectively. These mAP scores indicate enhanced detection accuracy across various Intersection over Union (IoU) thresholds, reflecting robust model performance.

### Summary
Overall, the model shows strong convergence and balanced performance across training and validation data. Declining loss curves and rising precision, recall, and mAP scores indicate effective learning and minimal overfitting, highlighting the model's readiness for deployment.







