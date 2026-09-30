# Computer-Vision-Canny-Edge-Detection

## Overview

This project demonstrates edge detection techniques in Digital Image Processing using three popular operators:

- Sobel Edge Detection
- Prewitt Edge Detection
- Canny Edge Detection

The program reads a grayscale image, applies each edge detection method, and displays the results for comparison.

## Objectives

- To understand the concept of edge detection.
- To implement Sobel and Prewitt operators using convolution kernels.
- To apply the Canny edge detection algorithm.
- To compare the outputs of different edge detection techniques.

## Technologies Used

- Python 3.x
- OpenCV
- NumPy
- Matplotlib

## Required Libraries

Install the required libraries using:

```bash
pip install opencv-python numpy matplotlib
```

## Project Structure

```text
Computer-Vision-Canny-Edge-Detection/
│
├── 23016CV6.py
├── image16.jpg
├── output.png
└── README.md
```

## Algorithms Used

### 1. Sobel Edge Detection

The Sobel operator detects edges by calculating image gradients in the horizontal and vertical directions.

#### Sobel X

```text
[-1   0   1]
[-2   0   2]
[-1   0   1]
```

#### Sobel Y

```text
[-1  -2  -1]
[ 0   0   0]
[ 1   2   1]
```

#### Gradient Magnitude

```text
G = √(Gx² + Gy²)
```

The Sobel operator is useful for detecting edges and changes in intensity in an image.

### 2. Prewitt Edge Detection

The Prewitt operator detects edges using horizontal and vertical convolution kernels.

#### Prewitt X

```text
[-1   0   1]
[-1   0   1]
[-1   0   1]
```

#### Prewitt Y

```text
[-1  -1  -1]
[ 0   0   0]
[ 1   1   1]
```

#### Gradient Magnitude

```text
G = √(Px² + Py²)
```

The Prewitt operator is used to detect horizontal and vertical edges in an image.

### 3. Canny Edge Detection

Canny Edge Detection is a multi-stage edge detection algorithm.

The main steps are:

1. Noise Reduction
2. Gradient Calculation
3. Non-Maximum Suppression
4. Double Thresholding
5. Edge Tracking by Hysteresis

Example:

```python
canny_result = cv2.Canny(img, 100, 200)
```

## Methodology

The program follows these steps:

1. Read the input image.
2. Convert the image into grayscale.
3. Apply the Sobel operator.
4. Apply the Prewitt operator.
5. Apply the Canny edge detection algorithm.
6. Display the original image and the edge detection results.

## How to Run

### Step 1

Place the input image in the project folder.

```text
image16.jpg
```

### Step 2

Install the required libraries:

```bash
pip install opencv-python numpy matplotlib
```

### Step 3

Run the Python program:

```bash
python 23016CV6.py
```

## Output

The program displays a comparison of:

- Original Image
- Sobel Edge Detection Result
- Prewitt Edge Detection Result
- Canny Edge Detection Result

### Output Image

![Edge Detection Output](output.png)

## Applications

Edge detection techniques are widely used in:

- Object Detection
- Image Segmentation
- Medical Image Processing
- Face Recognition
- Autonomous Vehicles
- Computer Vision
- Image Analysis

## Learning Outcomes

After completing this project, the following concepts can be understood:

- Image gradients
- Convolution operations
- Sobel edge detection
- Prewitt edge detection
- Canny edge detection
- Comparison of different edge detection techniques
- Applications of edge detection in Computer Vision

## Result

The Sobel, Prewitt, and Canny edge detection techniques were successfully applied to the input image. The resulting edge maps demonstrate the differences between the three edge detection methods.

## Conclusion

Edge detection is an important technique in Digital Image Processing and Computer Vision. Sobel and Prewitt operators use convolution kernels to detect intensity changes, while Canny uses multiple processing stages to produce a refined edge map. These techniques are useful for identifying important boundaries and structures within images.

## Author

**Muvva Avinash**

B.Tech – Data Science

Computer Vision Laboratory Project
