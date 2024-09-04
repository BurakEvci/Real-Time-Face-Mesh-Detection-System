# Real-Time Face Mesh Detection System
This project is a real-time computer vision application that detects and visualizes facial landmarks using a webcam or a video file. It uses MediaPipe's Face Mesh solution to map 468 facial landmarks, providing detailed and dynamic facial analysis.

![image](https://github.com/user-attachments/assets/df34608b-2d71-4b88-adcd-bb3d150790ec)

## 1. Real-Time Face Detection with OpenCV
The application captures live video feed from a webcam (cv2.VideoCapture(0)) or can be adapted to work with video files.

The video frames are processed in real-time, making the system suitable for interactive applications such as facial analysis and augmented reality.
## 2. Face Mesh Detection with MediaPipe
The application uses MediaPipe’s Face Mesh solution, which is capable of detecting and tracking up to 468 landmarks per face.

The FaceMeshDetector class is used to initialize and manage the detection process, allowing customization of detection parameters like the maximum number of faces, detection confidence, and tracking confidence.
## 3. Drawing and Visualizing Facial Landmarks
The detected landmarks are drawn on the face using the mpDraw module from MediaPipe, with custom drawing specifications such as color, thickness, and circle radius.

The application displays the landmarks in real-time, providing immediate visual feedback.
## 4. Extracting Landmark Positions
For each detected face, the system calculates the positions of the landmarks relative to the image dimensions and prints their coordinates.

This feature is useful for further processing or integrating with other systems that require precise facial landmark data.
## 5. Frame Rate Display
The application calculates and displays the frames per second (FPS) on the screen, providing feedback on the real-time performance of the detection system.
## 6. Application Flow
Initialization: The system initializes the camera and sets up the face mesh detector with specified parameters.

Face Detection: The application processes each video frame to detect facial landmarks.

Landmark Visualization: Detected landmarks are drawn on the image for visualization.

Position Extraction: Landmark coordinates are extracted and can be used for further analysis or applications.

Performance Monitoring: The FPS value is displayed to monitor the system’s real-time performance.
## Use Case
This project can be used in applications such as facial recognition, augmented reality, emotion detection, or any other scenario that requires detailed facial landmark detection and tracking. It is ideal for developers looking to create interactive, face-driven applications.
