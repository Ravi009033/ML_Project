#Project Overview: Face Recognition using OpenCV + NumPy
This project implements a basic face recognition system using a combination of:

- Haar Cascade for face detection
- NumPy arrays to store face data
- K-Nearest Neighbors (KNN) for classification

#📌 Project Breakdown
Here’s how project is likely structured:
1. Face Data Collections

- Captures face images from webcam using OpenCV.
- Uses Haar Cascade (haarcascade_frontalface_alt.xml) to detect faces.
- Stores the largest face per frame, resized to 100x100 pixels.
- Every 10th frame is stored to avoid redundancy.
- Data is saved in .npy format using NumPy, shaped as (N, 30000) (flattened 100×100×3 image).

2. Loading and Preparing the Training Dataset
   
- Loads all saved .npy files from the dataset folder.
- Assigns a unique label to each person.
- Combines all data and labels into a final training set.

3. Face Recognition using KNN
For each new frame from the webcam:

- Detects the face.
- Extracts and resizes the region of interest (ROI).
- Flattens and feeds it into a custom KNN classifier.
- Finds the most similar face data and displays the predicted name on screen.

 4. Live Testing
    
- Uses the webcam to continuously detect and recognize faces in real-time.
- Shows the frame with a rectangle and the predicted label (person's name). 

#🧠 KNN Logic:

- Compute Euclidean distance from input face to all training faces.
- Sort and pick the top K.
- Return the label with the majority votes.

 #🧪 Sample Output 
 
 When you run the final face recognition:
- It draws rectangles around detected faces.
- It prints the name of the recognized person (if match found).
- Exits on pressing 'q'.
   
