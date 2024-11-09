# Machine Problem 5: Object Detection and Recognition using YOLO
---

## Objective

The purpose of this task is to implement real-time object detection using the YOLO (You Only Look Once) model, with hands-on experience in loading pre-trained models, processing images, and visualizing results.

## Table of Contents

- [Tasks](#tasks)
  - [Task 1: Model Loading](#task-1-model-loading)
  - [Task 2: Image Input](#task-2-image-input)
  - [Task 3: Object Detection](#task-3-object-detection)
  - [Task 4: Visualization](#task-4-visualization)
  - [Task 5: Testing](#task-5-testing)
  - [Task 6: Performance Analysis](#task-6-performance-analysis)
- [Key Observations](#key-observations)
- [Conclusion](#conclusion)

---

## Tasks

### Task 1: Model Loading

- **Objective**: Initialize and load a pre-trained YOLO model using OpenCV’s DNN module.
- **Steps**:
  1. Load YOLO configuration and weights.
  2. Map object class names from the COCO dataset.
  3. Set up YOLO for CPU processing.

### Task 2: Image Input

- **Objective**: Load and display an image.
- **Steps**:
  1. Define a function to load an image from a specified path.
  2. Ensure error handling in case of missing images.

### Task 3: Object Detection

- **Objective**: Use YOLO to detect objects within an image.
- **Steps**:
  1. Preprocess the image to YOLO’s input dimensions (416x416).
  2. Run a forward pass to detect objects and filter by confidence threshold.

### Task 4: Visualization

- **Objective**: Display detected objects with bounding boxes and labels.
- **Steps**:
  1. Generate random colors for each class.
  2. Draw bounding boxes and add labels for each detection.
  3. Display the annotated image.

### Task 5: Testing

- **Objective**: Test YOLO on multiple images to evaluate performance.
- **Steps**:
  1. Run object detection on at least three different images.
  2. Display each result in a subplot for comparison.

### Task 6: Performance Analysis

- **Objective**: Analyze YOLO’s detection speed and accuracy.
- **Steps**:
  1. Calculate detection time and the number of objects detected per image.
  2. Compute average detection time and count across all test images.
  3. Summarize results for insights into YOLO’s efficiency and capabilities.

## Key Observations

- **YOLO Efficiency**: Performs detection in a single pass, ideal for real-time applications.
- **Detection Speed**: Consistently quick, with average detection times calculated across multiple images.
- **Object Detection Accuracy**: Handles diverse object classes effectively, though accuracy may vary with object complexity and image quality.

## Conclusion

The YOLO model is highly efficient for real-time object detection, providing accurate results across various images with multiple object classes. The single-pass architecture allows for quick detection times, making it suitable for applications requiring immediate responses. This project demonstrates YOLO’s robustness and efficiency, highlighting its capability in both speed and accuracy.

---
