# Exercise 2: Feature Extraction and Object Detection

---

## Exercise Overview

This exercise demonstrates the use of various feature extraction and object detection techniques, including SIFT, SURF, and ORB. The exercise explores keypoint detection, feature matching, and real-world applications like image stitching.

## Table of Contents

- [Techniques](#techniques)
  - [SIFT Feature Extraction](#sift-feature-extraction)
  - [SURF Feature Extraction](#surf-feature-extraction)
  - [ORB Feature Extraction](#orb-feature-extraction)
  - [Feature Matching](#feature-matching)
  - [Image Stitching using Homography](#image-stitching-using-homography)
  - [Combining Feature Extraction Methods](#combining-feature-extraction-methods)
- [Conclusion](#conclusion)

---

## Techniques

### SIFT Feature Extraction

- **Task**: Detect keypoints in an image using SIFT (Scale-Invariant Feature Transform).
- **Steps**:
  1. Load an image.
  2. Detect and compute keypoints and descriptors.
  3. Visualize keypoints on the image.
- **Result**: Keypoints are displayed as distinctive points in the image.

### SURF Feature Extraction

- **Task**: Detect keypoints using SURF (Speeded-Up Robust Features) for faster detection.
- **Steps**:
  1. Load a different image.
  2. Apply SURF to detect keypoints and compute descriptors.
  3. Visualize the detected keypoints.
- **Result**: Keypoints detected by SURF are highlighted, focusing on speed and efficiency.

### ORB Feature Extraction

- **Task**: Detect keypoints using ORB (Oriented FAST and Rotated BRIEF) for efficient real-time applications.
- **Steps**:
  1. Apply ORB to another image.
  2. Detect keypoints and compute descriptors.
  3. Display the detected keypoints.
- **Result**: ORB provides a fast and lightweight alternative for keypoint detection.

### Feature Matching

- **Task**: Match features between two images using descriptors from SIFT, SURF, or ORB.
- **Steps**:
  1. Detect keypoints and descriptors in two images.
  2. Use Brute-Force or FLANN Matcher to find matches.
  3. Visualize matched keypoints on both images.
- **Result**: Matched points are displayed, showing corresponding features across images.

### Image Stitching using Homography

- **Task**: Use homography to align two images based on matched features.
- **Steps**:
  1. Match keypoints between two images.
  2. Compute the homography matrix.
  3. Apply homography to align one image with the other.
- **Result**: Aligned images, demonstrating a foundational technique in panorama stitching.

### Combining Feature Extraction Methods

- **Task**: Use both SIFT and ORB for robust feature extraction and matching.
- **Steps**:
  1. Detect features using SIFT and ORB in two images.
  2. Match features using each method and combine results.
  3. Visualize the combined matches.
- **Result**: Side-by-side comparison showing matches from each algorithm and combined results.

## Conclusion

This exercise showcases the capabilities of SIFT, SURF, and ORB in feature extraction, along with their applications in feature matching and image alignment. Each algorithm presents unique strengths, such as SIFT's accuracy, SURF's balanced speed, and ORB's efficiency for real-time applications. Homography aids in practical applications like image stitching, demonstrating the power of feature extraction in computer vision.

---
