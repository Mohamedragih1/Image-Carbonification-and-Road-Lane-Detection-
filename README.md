# Image Cartoonification and Road Lane Detection

## Overview
This assignment consists of two parts focused on fundamental computer vision tasks:

1. **Image Cartoonification**: Transform real-world images into cartoon-like visuals using edge detection and image processing techniques.
2. **Road Lane Detection**: Detect road lanes in images using the Hough Transform.

The assignment is a practical application of image processing concepts, incorporating edge detection, smoothing, and transformations to achieve the desired outputs.

---

## Part I: Applying Image Processing Filters for Image Cartoonification

### Objectives
- Generate a black-and-white sketch from an image.
- Produce a color painting with an edge-preserving filter.
- Combine the sketch and the painting to achieve a cartoon effect.

### Steps
1. **Black-and-White Sketch**:
   - Apply **noise reduction** using a Median filter to preserve edges.
   - Perform **edge detection** with a Laplacian filter.
   - Enhance edges using binary thresholding.

2. **Color Painting and Cartoon Effect**:
   - Use a **bilateral filter** to smooth flat regions while preserving edges.
   - Combine the sketch and the smoothed painting to create the cartoon effect.

### Key Techniques
- **Edge Detection**: Laplacian filter.
- **Noise Reduction**: Median filter.
- **Edge-Preserving Smoothing**: Bilateral filter.

---

## Part II: Road Lane Detection Using Hough Transform

### Objectives
- Detect road lanes in an image using Hough Transform.
- Identify and highlight the region of interest (ROI) to focus on road edges.

### Steps
1. **Image Smoothing**:
   - Reduce noise using a 2D Median filter.

2. **Edge Detection**:
   - Apply **Canny edge detection** with high thresholds to minimize noise.

3. **Region of Interest (ROI)**:
   - Mask irrelevant edges by defining a polygonal region around the road.

4. **Hough Transform**:
   - Accumulate points in \((\rho, \theta)\)-space.
   - Identify line parameters using peaks in the accumulator array.
   - Refine coordinates through non-maximum suppression for post-processing.

---

## References
- **Faculty of Engineering, Alexandria University**
- **Supervisors**: 
  - Dr. Marwan Torki
  - Eng. Shereen Elkordi
  - Eng. Ismail Elyamany

