# 🚗 Lane Detection using OpenCV
This project performs lane line detection on road images and videos using computer vision techniques with OpenCV. 
It highlights lane lines and fills the lane area with green color, providing a visual representation of the drivable area.


## 📌 Features

- Edge detection using Canny
- Region of Interest (ROI) masking
- Line detection using Hough Transform
- Lane line extrapolation
- Lane area filling with green overlay


## 🛠️ Requirements

Install required Python packages:
bash''' pip install numpy matplotlib opencv-python

# 🚀 How to Run
- Clone or download this repository.
- Place your road image in the working directory.
- Open and run the Jupyter Notebook:
jupyter notebook "lane detection from image.ipynb"

- Follow the code cells in sequence to:
  - Load the image
  - Detect lane lines
  - Overlay the filled lane area in green

# 🧠 Algorithm Overview

- Grayscale & Blur: Convert to grayscale and apply Gaussian blur to reduce noise.
- Canny Edge Detection: Identify sharp changes in pixel intensity.
- ROI Masking: Focus on the road area using a polygonal mask.
- Hough Transform: Detect straight lines representing lane boundaries.
- Lane Filling: Draw a green polygon between left and right lines to visualize the lane.


  
