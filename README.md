
#Automatic Number Plate Recognition (ANPR) using EasyOCR & OpenCV

This project implements an **Automatic Number Plate Recognition (ANPR)** system using **Python**, **OpenCV**, and **EasyOCR**.
It detects a vehicle’s license plate from an image, extracts the plate region, and recognizes the text using Optical Character Recognition (OCR).

##  Features

* License plate detection using **image processing**
* Noise reduction with **bilateral filtering**
* Edge detection using **Canny**
* Contour-based plate localization
* Text extraction using **EasyOCR**
* Works on real-world vehicle images


## 🛠️ Technologies Used

* Python
* OpenCV (`cv2`)
* EasyOCR
* NumPy
* Matplotlib
* imutils





## Pipeline

1. **Image Preprocessing**

   * Convert image to grayscale
   * Apply bilateral filter to reduce noise

2. **Edge Detection**

   * Use Canny edge detector to highlight plate edges

3. **Contour Detection**

   * Find contours and identify quadrilateral regions
   * Select the contour most likely to be a number plate

4. **Masking & Cropping**

   * Extract the license plate region

5. **OCR (Text Recognition)**

   * Use EasyOCR to read license plate text

6. **Visualization**

   * Draw bounding box and display recognized text
