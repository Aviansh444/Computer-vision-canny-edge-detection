# Computer-vision-canny-edge-detection
Overview
This project demonstrates edge detection techniques in Digital Image Processing using three popular operators:

Sobel Edge Detection
Prewitt Edge Detection
Canny Edge Detection
The program reads a grayscale image, applies each edge detection method, and displays the results for comparison.

Objectives
To understand the concept of edge detection.
To implement Sobel and Prewitt operators manually using convolution kernels.
To apply the Canny edge detection algorithm.
To compare the outputs of different edge detection techniques.
Technologies Used
Python 3.x
OpenCV
NumPy
Matplotlib
Required Libraries
Install the required libraries using:

pip install opencv-python numpy matplotlib
Project Structure
Edge-Detection/
│
├── 23016CV6.py
├── input_image.jpg
├── README.md
└── output
Algorithms Used
1. Sobel Edge Detection
The Sobel operator calculates image gradients in horizontal and vertical directions using the following kernels:

Sobel X

[-1  0  1]
[-2  0  2]
[-1  0  1]
Sobel Y

[-1 -2 -1]
[ 0  0  0]
[ 1  2  1]
Gradient Magnitude:

G = √(Gx² + Gy²)
2. Prewitt Edge Detection
The Prewitt operator detects edges using the following kernels:

Prewitt X

[-1  0  1]
[-1  0  1]
[-1  0  1]
Prewitt Y

[-1 -1 -1]
[ 0  0  0]
[ 1  1  1]
Gradient Magnitude:

G = √(Px² + Py²)
3. Canny Edge Detection
Canny Edge Detection consists of:

Noise Reduction
Gradient Calculation
Non-Maximum Suppression
Double Thresholding
Edge Tracking by Hysteresis
Example:

canny_result = cv2.Canny(img, 100, 200)
How to Run
Place an image named image16.jpg in the project folder.
Run the Python script:
python 23016CV6.py
The program will display:

Original Image
Sobel Edge Detection Result
Prewitt Edge Detection Result
Canny Edge Detection Result
Expected Output
The output window shows a comparison of:

+-------------------+-------------------+
| Original Image    | Sobel Result      |
+-------------------+-------------------+
| Prewitt Result    | Canny Result      |
+-------------------+-------------------+
Applications
Object Detection
Image Segmentation
Medical Image Processing
Face Recognition Systems
Autonomous Vehicles
Computer Vision Projects
Learning Outcomes
After completing this project, users will be able to:

Understand image gradients.
Perform convolution operations manually.
Compare different edge detection methods.
Apply edge detection techniques in Computer Vision applications.
Author
Muvva Avinash

B.Tech – Computer Science / Data Science

Computer Vision Laboratory Project
