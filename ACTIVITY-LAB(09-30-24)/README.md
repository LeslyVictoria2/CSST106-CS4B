# Activity Lab: Frame Extraction and Analysis

This activity lab focuses on extracting frames from a video using OpenCV and performing further analysis on each frame. Below are the steps, including code and explanations for each part of the process.

### Setup

First, we need to install the OpenCV library for image processing.

```python
!pip install opencv-python
```

### Mounting Google Drive

To access files stored in Google Drive, we mount the drive to Colab. This allows us to use videos or images stored in the drive.

```python
from google.colab import drive
drive.mount('/content/drive')
```

### Import Libraries and Define Functions

Here, we import necessary libraries and define a function to extract frames from the video. This function captures frames at a specified frame rate.

```python
import cv2
import os

# Function to extract frames
def extract_frames(video_path, output_folder, fps=2):
    # Open the video file
    video_capture = cv2.VideoCapture(video_path)

    # Get the frames per second (fps) of the video
    video_fps = video_capture.get(cv2.CAP_PROP_FPS)

    # Calculate the interval between frames to capture based on video fps and desired fps
    frame_interval = int(video_fps / fps)

    # Create the output folder if it doesn't exist
    if not os.path.exists(output_folder):
        os.makedirs(output_folder)

    frame_number = 0
    extracted_frame_number = 0

    while True:
        # Read the next frame
        success, frame = video_capture.read()

        # Break the loop when the video ends
        if not success:
            break

        # Save the frame if it's the desired frame (every frame_interval)
        if frame_number % frame_interval == 0:
            frame_filename = os.path.join(output_folder, f"frame_{extracted_frame_number}.jpg")
            cv2.imwrite(frame_filename, frame)
            extracted_frame_number += 1

        frame_number += 1

    # Release the video capture object
    video_capture.release()
    print(f"Extracted {extracted_frame_number} frames to '{output_folder}'.")
```

### Explanation

- **Function Definition**: `extract_frames()` function takes in a video path, an output folder, and a frame rate at which frames are extracted.
- **Frame Interval Calculation**: This determines how often frames are saved based on the original video frame rate.
- **Loop and Save**: The loop saves frames at intervals to achieve the desired frame rate, releasing resources at the end.
