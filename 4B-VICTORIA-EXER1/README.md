# **EXERCISE 1**
## Blurring Techniques and Edge Detection Techniques (Comparison)
## **Lesly-Ann B. Victoria from BSCS-4B**

### **IMAGES:**
![image](https://github.com/user-attachments/assets/feb6406b-af1d-4dcd-84ef-2cc74d79a92d)

- This is the 2x2 picture I used in making these exercises.

![image](https://github.com/user-attachments/assets/fe9c0a4e-92f8-4335-82cf-2037b9415198)

- This is the scaled image and rotated image. The first image is a scaled version, reduced to 50% of its original size, which decreases the dimensions while maintaining the image's proportions. The second image has been rotated by 45 degrees, altering its orientation but preserving the content of the original image.

## **BLURRING TECHNIQUES:**
- Gaussian blur is often used to reduce noise and soften edges. It's a popular choice for general purpose blurring.
- Median blur is particularly effective at removing salt-and-pepper noise (random black and white pixels). It preserves edges better than Gaussian blur.
- Bilateral filter is useful for preserving edges while reducing noise. It's a good choice for images with fine details.
- Box filter is a simple blurring technique that can be used to smooth out noise. However, it can also blur edges.
- Motion blur can be used to create artistic effects or to simulate real-world motion.
- Unsharp mask is often used to enhance image details and make them appear sharper.

### Images:
![image](https://github.com/user-attachments/assets/72cd04c9-0580-4e3e-943a-6651a4855bad)

1. Gaussian Blur - This image shows the effect of Gaussian Blur, where the picture has been blurred by applying a Gaussian function. This technique results in a smooth blur, evenly distributing the blur effect across the image, which softens the sharp details.
2. Median Blur - The second image demonstrates Median Blur, which reduces noise by replacing each pixel's value with the median value of the neighboring pixels. This technique creates a soft, more blended look, but can maintain edges better than other types of blur.
3. Bilateral Filter - This filter preserves the edges while blurring the image, as seen in the third image. It smoothes regions of similar color or brightness but keeps the distinct boundaries of objects intact, making the subject's facial features clearer compared to other blurring techniques.
4. Box Blur - In the fourth image, Box Blur has been applied, resulting in a uniform and simple blur effect. The image appears as if a square filter has been averaged over each pixel in a grid pattern, creating a slightly less sophisticated blur.
5. Motion Blur - The fifth image demonstrates Motion Blur, simulating the effect of moving the camera or subject during the shot. This results in streaks or lines that give the impression of movement, with the blur following a specific direction.
6. Unsharp Mask - The final image utilizes the Unsharp Mask technique, which sharpens the image by enhancing the contrast of edges. It gives a clearer, more defined look compared to the other techniques, with the subject's facial features appearing sharper and more prominent.

![image](https://github.com/user-attachments/assets/f11580bb-a738-4f93-a704-45426ca35b1e)

*This Table 1 above compares different blurring techniques based on their ability to blur, reduce noise, preserve edges, create artistic effects, and sharpen images. Gaussian Blur is commonly used for blurring and noise reduction but doesn't contribute to edge preservation and artistic effects or sharpening. Median Blur excels at noise reduction and edge preservation while also providing basic blurring. Bilateral Filter is unique in that it blurs while preserving edges, noise reduction and is often used in artistic effects such as cartoonizing images. Box Blur is a simple technique that only blurs, without offering noise reduction, edge preservation, artistic effects or sharpening. Motion Blur simulates the effect of moving objects and is mainly used for artistic purposes. Finally, the Unsharp Mask is a sharpening tool rather than a blurring method, enhancing edge contrast to sharpen images.*

## **EDGE DETECTION TECHNIQUES:**
- Sobel edge detection is a simple and computationally efficient method. It's sensitive to noise and can produce double edges.
- Laplacian edge detection is less sensitive to noise than Sobel edge detection but can be more susceptible to noise. It may also produce multiple edges for a single edge.
- Prewitt edge detection is also a simple and computationally efficient method. It's like Sobel edge detection in terms of sensitivity to noise and the potential for double edges.
- Canny edge detection is considered one of the most robust edge detection algorithms. It's less sensitive to noise than Sobel and Laplacian, and it can produce thin, continuous edges.
