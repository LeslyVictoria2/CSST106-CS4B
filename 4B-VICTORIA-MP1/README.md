# **MACHINE PROBLEM 1**
## Exploring the Role of Computer Vision and Image Processing in AI

## **Lesly-Ann B. Victoria from BSCS-4B**

## **Presentation Development:**
https://github.com/user-attachments/assets/09c88255-4c11-4400-a652-8d49e25cd182

https://github.com/user-attachments/assets/72cb9beb-8a7f-4ae4-9418-7cd8a5d42daa

## **Introduction to Computer Vision and Image Processing:**

### **Computer Vision**
- A branch of computer science that empowers machines to see, recognize and process images just like humans.
- A field of AI that enables computers to interpret and make decisions based on visual data, such as images and videos.
- It uses artificial intelligence and machine learning (AI/ML) to process this data accurately for object identification and facial recognition, as well as classification, recommendation, monitoring, and detection.

### **How AI Systems Process Visual Information**
AI systems use computer vision algorithms to process visual information. The process involves capturing images through sensors or cameras, pre-processing these images to enhance their quality, and then using models and algorithms to analyze the visual data.

### **Role of Image Processing in AI systems**
- AI image processing uses artificial intelligence to analyze and enhance images.
- It involves tasks like pattern recognition, object detection, and image classification.
- Core technologies include deep learning, neural networks, and machine learning algorithms.
- Revolutionizes healthcare, security, and entertainment by automating complex tasks and improving accuracy.

## **Types of Image Processing Techniques:**

### **1. Filtering**
- A technique used to enhance the quality of images.
- It involves the application of mathematical operations to an image to extract important features, remove noise, or blur images.
Filtering operations such as blurring, sharpening and noise reduction are applied to images using convolution. Convolution involves sliding a filter or kernel over an image and performing mathematical operations on each pixel. This process enables various improvements such as anti-aliasing, edge detection and texture removal.
#### Example: A Gaussian filter can smoothen an image, removing unwanted noise, while sharpening filters can enhance the edges and details in an image.

### **2. Edge Detection**
- A technique used for identifying and locating the boundaries or edges of objects in an image.
- It is used to identify and detect the discontinuities in the image intensity and extract the outlines of objects present in an image.
Edge detection algorithms identify image boundaries and important transitions. They emphasize areas where the intensity changes quickly, such as edges, curves or contours. Edge detection plays an important role in object detection, shape analysis and feature extraction. Popular edge detection algorithms are Canny edge detector and Sobel operator.
#### Example: Canny Edge Detection, Sobel Edge Detection, Laplacian Edge Detection, Prewitt Edge Detection.

### **3. Segmentation**
- A technique used to separate objects, boundaries, or structures within the image for more meaningful analysis.
- It involves partitioning a digital image into multiple segments (regions or objects) to simplify and analyze an image by separating it into meaningful components.
Image segmentation involves dividing an image into several distinct regions based on their visual characteristics. This technique allows you to separate objects from the background or divide the image into significant regions. Common segmentation methods include thresholding, region growing, clustering, and graph-based algorithms. Image segmentation is an essential step in many computer vision tasks, including object detection, image annotation, and semantic understanding.
#### Example: Object Detection, Medical Imaging and Image Recognition.

## **Case Study Overview:**

### **Autonomous Vehicles**
- A driverless vehicle is one that is able to operate itself and perform necessary functions without any human intervention, through the ability to sense its surroundings.
- Utilizes a fully automated driving system in order to allow the vehicle to respond to external conditions that a human driver would manage.
### **How Image Processing used in Autonomous Vehicles**
- Autonomous vehicles rely heavily on image processing to navigate and make real-time decisions.
- The use of cameras and sensors to capture images of their surroundings, which are then processed using computer vision techniques. These techniques help the vehicle detect obstacles, recognize traffic signs, identify lanes, and interpret road conditions.
- The images captured from the autonomous car are processed by the proposed system which is used to control the autonomous vehicle.
  
## **PROBLEM: Lane Detection in Autonomous Vehicles**

## **My Image Processing Implementation:**
- Problem in autonomous vehicles is detecting the lane boundaries to ensure the vehicle stays within its lane. Edge detection is a key technique used to solve this problem.
- I use Canny Edge Detection technique to detect lane boundaries in captured images from the car.
- The lane detection model helps the AI system keep the vehicle within its lane, plan safe paths, and navigate efficiently, enhancing overall driving safety.

### **Lane Detection Systems for Autonomous Vehicles**
### **Step 1:**
The first step is to capture an image from the car camera to implement image processing.

![image](https://github.com/user-attachments/assets/7bcf99d9-d662-45c2-ae93-760a96374a6c)

### **Step 2:**
Next, I used Google Colab to implement the image processing.

![download (1)](https://github.com/user-attachments/assets/6bab493c-c3f6-4811-9e01-b9d60920f1d6)

### **Step 3:**
The cv2, numpy, and matplotlib.pyplot are imported. These libraries are essential for image processing (cv2), numerical operations (numpy), and visualizing results (matplotlib).

![Screenshot 2024-09-04 201201](https://github.com/user-attachments/assets/6b56bf05-677b-4877-bfd8-5d0b7e736d22)

### **Step 4:**
The image file 'image.jpg' is read using cv2.imread. The image is then converted from BGR (OpenCV's default) to RGB for proper display with matplotlib, and shown with a title "Original Captured Image".

![Screenshot 2024-09-04 201636](https://github.com/user-attachments/assets/1e42386f-d590-42d7-ba4e-8695bafcdaf7)

**Result:**

![image](https://github.com/user-attachments/assets/079095ef-a227-4a73-8e5d-7723a9ffdafb)

### **Step 5:**
The color image is converted to grayscale using cv2.cvtColor, reducing it to a single channel, which is easier to process for edge detection. The grayscale image is displayed with a title "Grayscale Image".

![Screenshot 2024-09-04 201907](https://github.com/user-attachments/assets/1c944df9-134c-4ae7-8a74-615872367049)

**Result:**

![image](https://github.com/user-attachments/assets/b1b9a793-54a5-4546-a12a-d64c1aa87f9b)

### **Step 6:**
A Gaussian Blur is applied to the grayscale image using cv2.GaussianBlur, which helps reduce noise and detail. This step smooths the image, making edge detection more accurate. The blurred image is displayed with the title "Gaussian Filter Image".

![Screenshot 2024-09-04 201929](https://github.com/user-attachments/assets/778c78dc-d3a0-47b8-8d10-8b432c182162)

**Result:**

![image](https://github.com/user-attachments/assets/aa1325d6-cf7a-4022-ba93-f14baa3eeec0)

### **Step 7:**
Canny Edge Detection is applied to the blurred image using cv2.Canny, detecting edges by looking for areas of rapid intensity change. The detected edges are shown with the title "Canny Edge Detection".

![Screenshot 2024-09-04 201956](https://github.com/user-attachments/assets/c4e97e37-f8ec-47fa-a006-db250f86dc7d)

**Result:**

![image](https://github.com/user-attachments/assets/76ecd780-1658-4841-86e5-f4499abec0d5)

### **Step 8:**
A polygonal mask is created to focus on a specific region of interest (ROI), typically where lane lines might appear. The ROI is filled with white (255), and applied to the edge-detected image using cv2.bitwise_and, highlighting edges only within this region.

![Screenshot 2024-09-04 202021](https://github.com/user-attachments/assets/197ba03f-de4b-4823-b0ef-c5f3fb9d15f9)

**Result:**

![image](https://github.com/user-attachments/assets/b3d1d78e-32ae-4ba3-a397-d7de8db72efc)

### **Step 9:**
The cv2.HoughLinesP detects lines in the masked edge image. The lines are drawn on a blank image (line_image) using cv2.line. The detected lines are shown in red, simulating lane markings. Then the line image is combined with the original captured image using cv2.addWeighted, highlighting the detected lanes over the original image. The final result is displayed with the title "Lane Detection Highlighted (Red Line)".

![Screenshot 2024-09-04 202045](https://github.com/user-attachments/assets/7236ac6e-353b-4491-9299-a037e13474f8)

**Result:**

![image](https://github.com/user-attachments/assets/37b2b314-4ab4-43a7-b98d-5a1bff47bd30)

## **Conclusion**
- The document underscores the importance of effective image processing in Artificial Intelligence (AI) as it enables AI systems to accurately interpret and analyze visual data. Techniques such as filtering, edge detection, and segmentation are vital in extracting meaningful information from images, which is essential for AI applications like autonomous vehicles, facial recognition, and medical imaging. In the case study on autonomous vehicles, the practical implementation of Canny Edge Detection demonstrated how image processing helps in ensuring lane detection, thereby enhancing driving safety.
- From this activity, I learned that effective image processing is foundational to the success of AI systems. It allows AI to perform complex tasks, such as object detection and scene understanding, with high precision. The hands-on experience of implementing edge detection for lane detection in autonomous vehicles highlighted how these techniques are applied in real-world scenarios, reinforcing the critical role of image processing in advancing AI technologies.

#### **Deep Learning Based Image Analysis**
- Deep learning uses neural networks to learn useful representations of features directly from data. For example, you can use a pre-trained neural network to identify and remove artifacts like noise from images.
- Deep Learning-Based Image Analysis is a major step forward in image processing, enabling AI to learn and improve its ability to analyze images directly from data.
- This approach increases the accuracy and efficiency of AI systems, making them more useful in different fields like healthcare, security, and self-driving cars.

#### **Potential Impact on Future AI Systems**
- The potential impact of this technique is immense, as it can greatly expand how AI can be applied to solve challenging visual tasks. For example, in my image processing implementation of lane detection in autonomous vehicles, the enhanced ability to process and interpret complex visual environments could make self-driving cars safer and more reliable, bringing us closer to widespread adoption.

## **Quotes**
*A computer is like a violin. You can imagine it, making beautiful music, but you have to learn how to play it.*
#### - Bill Gates


