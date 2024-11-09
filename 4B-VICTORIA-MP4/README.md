# Machine Problem 4: Feature Extraction and Image Matching in Computer Vision
---

## Overview

In this machine problem, various feature extraction and matching techniques are applied to analyze and compare images. Methods include SIFT, SURF, ORB, HOG, and Harris Corner Detection, with feature matching using FLANN and Brute-Force Matchers, as well as image segmentation via the Watershed algorithm.

## Objectives

1. Apply feature extraction methods (SIFT, SURF, ORB, HOG, and Harris Corner Detection).
2. Perform feature matching using Brute-Force and FLANN matchers.
3. Implement the Watershed algorithm for image segmentation.
4. Visualize keypoints and matches between images.
5. Evaluate the performance of different feature extraction methods.

## Tasks

### Task 1: Harris Corner Detection

- **Objective**: Detect corners in an image using the Harris Corner Detection method.
- **Function**: `def harris_corner_detection(image_path)`
- **Steps**:
  1. Load a grayscale image.
  2. Apply Harris Corner Detection.
  3. Display corners marked in red.
  
### Task 2: HOG Feature Extraction

- **Objective**: Extract Histogram of Oriented Gradients (HOG) features from an image.
- **Function**: `def hog_feature_extraction(image_path)`
- **Steps**:
  1. Load and convert an image to grayscale.
  2. Extract HOG features.
  3. Display the original and HOG visualization side-by-side.

### Task 3: ORB Feature Extraction and Matching

- **Objective**: Detect and match features between two images using ORB.
- **Function**: `def orb_feature_matching(image_path1, image_path2)`
- **Steps**:
  1. Load two grayscale images.
  2. Detect keypoints and compute descriptors.
  3. Match descriptors using FLANN and visualize matched keypoints.

### Task 4: SIFT and SURF Feature Extraction

- **Objective**: Detect keypoints using SIFT and SURF.
- **Function**: `def sift_and_surf_feature_extraction(image_path1, image_path2)`
- **Steps**:
  1. Load two images and resize for consistency.
  2. Apply SIFT and SURF to extract keypoints.
  3. Display detected keypoints for each method.

### Task 5: Feature Matching using Brute-Force Matcher

- **Objective**: Match ORB descriptors between two images using Brute-Force Matcher.
- **Function**: `def brute_force_feature_matching(image_path1, image_path2)`
- **Steps**:
  1. Extract ORB descriptors from both images.
  2. Match using Brute-Force Matcher.
  3. Display matched keypoints.

### Task 6: Image Segmentation using Watershed Algorithm

- **Objective**: Segment an image into distinct regions using the Watershed algorithm.
- **Function**: `def watershed_segmentation(image_path)`
- **Steps**:
  1. Load and convert the image to grayscale.
  2. Apply thresholding and morphological operations to identify background and foreground.
  3. Use Watershed for segmentation and display results.
