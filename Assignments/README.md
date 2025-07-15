# Image Processing Tasks

This README outlines the major tasks in the image processing project. Each task involves applying specific operations on images using Python. The tasks include enhancement, restoration, morphological operations, segmentation, recognition, feature representation, compression, and color analysis.

---

## 1. Image Enhancement

Pick an image of your choice to perform image enhancement.  
**Operations choices:** 
- Histogram equalization  
- Sharpening  
- Filtering  
- Denoising  

**Task:** Plot before and after images.

---

## 2. Image Restoration

Mask a certain region of your image to simulate a corrupted image.  
Then use some mathematical function to restore the pixels in that region.  

**Options:** 
- Interpolation  
- Convolutional filtering  

**Task:** Compare the restored image with the original image.

---

## 3. Morphological Operations

Pick a suitable image, then perform the following morphological operations:

- **Opening**  
- **Closing**

**Task:** Plot the original and processed images in a grid using subplots.

---

## 4. Segmentation

Pick a suitable image for segmentation.  
Use pre-trained models to perform:

- **Semantic Segmentation**  
- **Instance Segmentation**

**Models:**
- For BCT students: DeepLabV3  
- Other models: FCN, Mask R-CNN, U-Net, etc.

---

## 5. Image Recognition

Perform object detection on your image using pre-trained models of your choice.  

**Popular models:**
- SSD  
- Faster R-CNN  
- YOLO

---

## 6. Image Representation and Description

**i. Representation ("Where are the key features?")**  
Low-level features extracted to represent the structure of an image.  
**Example:** Edge detection, key-point detection, etc.

**ii. Description ("What those features look like numerically?")**  
Quantitative interpretation of those features.  
**Example:** SIFT descriptors, HOG vectors

**Task:**
- For *representation*, perform key-point detection using **SIFT** or **ORB**.
- For *description*, extract **SIFT** or **ORB** descriptors.  
- Print or summarize the descriptors as arrays.

---

## 7. Image Compression

Implement **2 image compression techniques** using Python (do not use online UI-based tools).  

**Options:**
- JPEG-style (DCT-based)
- PCA-based compression
- K-means-based color quantization

**Task:** Print the shape and total image size of both the original and compressed images.

---

## 8. Color Image Processing

**i. Channel Parsing:**  
Pick a colorful image, parse it into R, G, B channels. Plot the histograms of each channel.

**ii. Standard Deviation:**  
Use NumPy to compute and print the standard deviation of each channel.  
This estimates contrast—higher deviation means more visual information.

**iii. Thresholding and Evaluation:**  
Apply **OTSU thresholding** on each individual R, G, B channel.  

**Task:** Compare how well each channel separates foreground and background.  
Note: OTSU works best for **bimodal distributions** (histogram with 2 peaks).

**Objective Evaluation Methods:**

- **a. Plotting:**  
  - Plot the thresholded image  
  - Plot the histogram after thresholding  
  - Write insights using markdown

- **b. Entropy Calculation after Thresholding:**  
  - For bright/dark clean binary masks, entropy should be low  
  - Print entropy for each channel after thresholding  
  - Write markdown to discuss any cases where entropy fails to correctly estimate thresholding quality
