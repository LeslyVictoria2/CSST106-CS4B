# Exercise 3: Advanced Feature Extraction and Image Processing

**Course**: CSST106 - Perception and Computer Vision  
**Term**: 1st Semester, 2024-2025  
**University**: Laguna State Polytechnic University, Province of Laguna  
**Student**: Lesly-Ann B. Victoria  
**Section**: BSCS-4B  

---

## Exercise Overview

This exercise explores advanced feature extraction and image processing techniques using OpenCV, focusing on keypoint detection, feature matching, and image segmentation methods commonly applied in computer vision.

## Table of Contents

- [Techniques](#techniques)
  - [Harris Corner Detection](#harris-corner-detection)
  - [HOG Feature Extraction](#hog-feature-extraction)
  - [FAST Keypoint Detection](#fast-keypoint-detection)
  - [Feature Matching using ORB and FLANN](#feature-matching-using-orb-and-flann)
  - [Image Segmentation using Watershed Algorithm](#image-segmentation-using-watershed-algorithm)
- [Conclusion](#conclusion)

---

## Techniques

### Harris Corner Detection

- **Task**: Detect corners in an image using the Harris Corner Detection algorithm.
- **Steps**:
  1. Load an image and convert it to grayscale.
  2. Apply Harris Corner Detection.
  3. Highlight and display detected corners.
- **Result**: Corners are visualized, highlighting areas where edges intersect.

### HOG Feature Extraction

- **Task**: Extract features using HOG (Histogram of Oriented Gradients) for object structure representation.
- **Steps**:
  1. Load an image, ideally of a person or object.
  2. Convert it to grayscale.
  3. Apply HOG to extract and visualize gradient orientations.
- **Result**: Displays the gradient-based structure of objects, ideal for tasks like human detection.

### FAST Keypoint Detection

- **Task**: Detect keypoints quickly using FAST (Features from Accelerated Segment Test).
- **Steps**:
  1. Load and convert an image to grayscale.
  2. Detect keypoints using FAST.
  3. Visualize detected keypoints on the original image.
- **Result**: Keypoints are efficiently detected, suited for real-time applications.

### Feature Matching using ORB and FLANN

- **Task**: Match features between two images using ORB descriptors and FLANN-based matching.
- **Steps**:
  1. Load two images.
  2. Extract keypoints and descriptors using ORB.
  3. Match features with FLANN.
  4. Display the matched features.
- **Result**: Matched keypoints show corresponding features between two images, demonstrating object similarity across frames.

### Image Segmentation using Watershed Algorithm

- **Task**: Segment an image into distinct regions using the Watershed algorithm.
- **Steps**:
  1. Load and convert an image to grayscale.
  2. Apply a binary threshold.
  3. Use the Watershed algorithm to segment and label regions.
  4. Visualize segmented areas.
- **Result**: Regions in the image are segmented, useful for tasks like object separation and recognition.

## Conclusion

This exercise covers several advanced feature extraction and image processing methods, each with specific applications:
1. **Harris Corner Detection** - Finds intersection points of object edges.
2. **HOG Feature Extraction** - Extracts shape-based features for object recognition.
3. **FAST Keypoint Detection** - Efficient for real-time applications.
4. **ORB and FLANN Matching** - Compares features across images.
5. **Watershed Algorithm** - Segments overlapping objects in images.

Together, these techniques provide a foundation for diverse computer vision applications, including object detection, tracking, and image segmentation.

---
