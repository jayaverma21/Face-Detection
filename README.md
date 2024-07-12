# Face-Detection
This Python script utilizes OpenCV to detect faces from a webcam feed and provides several functionalities based on user input:

## Services Provided

### Detect and Display Image with Face Rectangle

- Detects a face in a single image frame from the webcam feed.
- Draws a rectangle around the detected face.
- Displays the modified image.

### Detect Faces in Live Video

- Continuously detects faces in the live video feed from the webcam.
- Draws rectangles around each detected face.
- Displays the annotated video feed.
- Press 'Enter' to exit.

### Detect Faces, Crop, and Display in Video

- Continuously detects faces in the live video feed from the webcam.
- Crops the detected face region.
- Resizes the cropped face to 200x200 pixels.
- Places the resized face in a fixed position within the video frame.
- Draws rectangles around each detected face.
- Displays the annotated video feed.
- Press 'Enter' to exit.

## Requirements

- Python 3.x
- OpenCV (cv2)

## Installation

1. Clone the repository:

   ```bash
   git clone <https://github.com/jayaverma21/Face-Detection>
2. Install the required libraries:

  
   ```bash
   pip install opencv-python
   
3. Download the Haar cascade XML file for face detection (myhaarcascade_frontalface_default.xml) and place it in the same directory as the script.

# Usage

+ Run the script and choose one of the following options by entering the corresponding number:
  + Option 1: Detect a face in a single image frame and display it with a rectangle.
  + Option 2: Detect faces continuously in the live video feed and display rectangles around each detected face.
  + Option 3: Detect faces continuously in the live video feed, crop each detected face, resize it, and display it in a fixed position within the frame.
+ Ensure your webcam is properly connected and accessible.

# Code Explanation
 + Option 1: Uses cv2.VideoCapture to capture a single frame, detects faces using CascadeClassifier, draws rectangles around each detected face using cv2.rectangle, and displays the modified frame.

 + Option 2: Uses cv2.VideoCapture to continuously capture frames from the webcam, detects faces in each frame, draws rectangles around detected faces, and displays the annotated video feed until 'Enter' is pressed to exit.

 + Option 3: Similar to Option 2, but additionally crops each detected face region, resizes it to 200x200 pixels, and places it in a fixed position within the video frame using array slicing and resizing operations.
