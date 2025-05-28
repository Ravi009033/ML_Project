# Real-Time Face Detection using OpenCV
This project uses OpenCV's Haar Cascade Classifier to detect human faces in real-time from a webcam feed.
Bounding boxes are drawn around detected faces, and the application exits gracefully when the user presses the `q` key.

## 🛠️ Requirements

- Python 3.x
- OpenCV

# Install dependencies:
pip install opencv-python

# 🧠 How It Works
- The webcam feed is captured using cv2.VideoCapture.
- Frames are converted to grayscale for efficient face detection.
- Haar cascade XML data (haarcascade_frontalface_alt.xml) is used to detect faces.
- Faces are highlighted with blue rectangles in real-time.
- When the user presses q, the script exits and cleans up resources.

