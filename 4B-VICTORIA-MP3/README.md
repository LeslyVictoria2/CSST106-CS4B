# Machine Problem 3: Feature Extraction and Object Detection
---

## Objective

The objective of this machine problem is to implement and compare three feature extraction methods: **SIFT**, **SURF**, and **ORB**. This task involves feature matching between two images and using Homography to align one image onto another. Performance in terms of accuracy and speed will be evaluated.

## Table of Contents

- [Problem Description](#problem-description)
- [Implementation Steps](#implementation-steps)
  - [Step 1: Load Images](#step-1-load-images)
  - [Step 2: Extract Keypoints and Descriptors](#step-2-extract-keypoints-and-descriptors)
  - [Step 3: Feature Matching](#step-3-feature-matching)
  - [Step 4: Image Alignment Using Homography](#step-4-image-alignment-using-homography)
  - [Step 5: Performance Analysis](#step-5-performance-analysis)
- [Submission Guidelines](#submission-guidelines)
- [Rubric](#rubric)

---

## Problem Description

1. **Feature Extraction**: Use SIFT, SURF, and ORB to extract keypoints and descriptors from two images of the same object or scene taken from different angles.
2. **Feature Matching**: Perform feature matching between the two images using both Brute-Force and FLANN Matchers.
3. **Image Alignment**: Use matched keypoints to compute a Homography matrix and align one image onto the other.
4. **Performance Comparison**: Evaluate SIFT, SURF, and ORB on feature matching accuracy, number of keypoints detected, and speed.

## Implementation Steps

### Step 1: Load Images

- **Task**: Load two images depicting the same scene or object from different perspectives.
- **Code**: Load images using OpenCV, resize as necessary, and display side-by-side for comparison.

### Step 2: Extract Keypoints and Descriptors

- **Task**: Apply SIFT, SURF, and ORB algorithms to detect keypoints and compute descriptors for each image.
- **Visualization**: Display the detected keypoints for each algorithm on both images, organized in a grid format to observe differences.
  
### Step 3: Feature Matching

- **Task**: Match descriptors between images using:
  - **Brute-Force Matcher**
  - **FLANN Matcher**
- **Visualization**: Display matching keypoints with lines connecting corresponding points between images, organized to compare SIFT, SURF, and ORB matches.

### Step 4: Image Alignment Using Homography

- **Task**: Compute a Homography matrix from matched keypoints using SIFT (or another method) and apply this transformation to align one image with the other.
- **Visualization**: Display the aligned and warped image alongside the original image to compare accuracy.

### Step 5: Performance Analysis

- **Task**:
  1. **Analyze Performance**:
     - Compare SIFT, SURF, and ORB in terms of:
       - Keypoint detection accuracy
       - Number of keypoints
       - Speed
     - Evaluate Brute-Force Matcher vs. FLANN Matcher for feature matching.
  2. **Report**:
     - Document observations and conclusions, including recommendations for the most effective feature extraction and matching technique.
