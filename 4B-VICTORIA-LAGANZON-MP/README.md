# Midterm Project: Feature Extraction and Object Detection

**Course**: CSST106 - Perception and Computer Vision  
**Term**: 1st Semester, 2024-2025  
**University**: Laguna State Polytechnic University, Province of Laguna  
**Students**: Lesly-Ann B. Victoria, Jonathan Q. Laganzon  
**Section**: BSCS-4B  

---

## Project Overview

This project explores feature extraction and object detection using two distinct approaches:

- **HOG-SVM (Histogram of Oriented Gradients with Support Vector Machine)**
- **YOLOv5 (You Only Look Once, Version 5)**

The primary objectives are to select and preprocess a dataset, implement the algorithms, train and evaluate models, and compare their performance on object detection tasks.

## Table of Contents

- [Dataset](#dataset)
- [Algorithms](#algorithms)
  - [HOG-SVM](#hog-svm)
  - [YOLOv5](#yolov5)
- [Implementation](#implementation)
  - [Data Preparation](#data-preparation)
  - [Model Training](#model-training)
  - [Evaluation](#evaluation)
- [Comparison and Discussion](#comparison-and-discussion)
- [Conclusion](#conclusion)
- [References](#references)

---

## Dataset

- **Dataset Used**: PASCAL VOC 2012
- **Links**:
  - [Pascal VOC Dataset on Google Drive](https://drive.google.com/drive/folders/1ULCGxid4QRqcQ35sLb4oRENUobmPLEhc?usp=sharing)
  - [Roboflow Link](https://public.roboflow.com/object-detection/pascal-voc-2012)

The PASCAL VOC dataset includes 20,000 images across 20 object categories, with well-defined bounding boxes and annotations suitable for object detection.

## Algorithms

### HOG-SVM

HOG-SVM is a traditional machine learning approach that uses histogram gradients to extract features, which are then classified by an SVM.

- **Advantages**: Efficient on simpler scenes and low computational power requirements.
- **Limitations**: Struggles with complex backgrounds and multi-scale detection.

### YOLOv5

YOLOv5 is a deep learning-based object detection model designed for real-time applications.

- **Advantages**: High accuracy, real-time detection capabilities.
- **Limitations**: Requires substantial computational power.

## Implementation

### Data Preparation

1. **Resizing** and **normalization** of images.
2. **Labeling** bounding boxes for YOLOv5.
3. Splitting the dataset into training and validation sets.

### Model Training

- **HOG-SVM**: Utilizes HOG feature extraction followed by training an SVM classifier.
- **YOLOv5**: Trained on labeled images, leveraging pretrained weights to expedite training.

### Evaluation

Metrics used for evaluation:
- **Accuracy**
- **Precision**
- **Recall**
- **Inference Speed**

## Comparison and Discussion

- **HOG-SVM**: Suitable for simpler, resource-constrained applications.
- **YOLOv5**: Better suited for complex, multi-object detection tasks.

## Conclusion

The HOG-SVM model is ideal for single-object detection tasks, while YOLOv5 excels in complex, multi-object detection scenarios. Each model's strengths and limitations emphasize the importance of aligning the algorithm with the task requirements and available resources.

## References

- GitHub Repository: [Person Detection](https://github.com/RashadGarayev/PersonDetection)
- [YOLOv5 Repository by Ultralytics](https://github.com/ultralytics/yolov5)

---
