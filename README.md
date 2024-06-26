﻿# FingerSketch-Interactive-Finger-based-Annotation-System-with-OpenCV

This Python script consists of two main parts: one for hand detection and tracking using the MediaPipe library, and the other for interactive drawing and annotation using OpenCV.

Hand Detection and Tracking (HandTrackingModule.py):

The handDetector class is defined to encapsulate hand detection and tracking functionality.
It utilizes the MediaPipe library (mediapipe) to detect and track hands in real-time from the webcam feed.
The class provides methods to find the positions of landmarks (key points) on detected hands and to determine the configuration of fingers (e.g., whether they are up or down).
Interactive Drawing and Annotation (VirtualPainter.py):

The script initializes parameters such as brush and eraser thickness, loads images from a specified folder (UI), and sets up a webcam capture.
It uses the handDetector class to detect and track hand movements in the webcam feed.
Depending on the hand gestures (e.g., finger positions), the script allows for interactive drawing and annotation on the canvas.
The canvas is represented as a NumPy array (imgCanvas) where drawing operations (e.g., lines and circles) are performed.
The script also implements a simple user interface (UI) for selecting different drawing colors using hand gestures.
Real-time performance metrics (e.g., frames per second) are displayed on the screen.
Description:

The script provides an interactive environment where users can draw and annotate on the screen using their fingers.
It leverages hand gestures to control drawing tools (e.g., selecting colors, switching between brush and eraser) and perform drawing actions (e.g., drawing lines and circles).
The canvas can be cleared by raising all fingers, providing a convenient way to start fresh drawings.
Users can switch between different drawing colors by positioning their fingers over predefined regions on the screen.
Performance metrics, such as frames per second (FPS), are displayed to monitor the real-time performance of the application.
Overall, the script offers a hands-on and intuitive way for users to engage in digital drawing and annotation tasks using their webcam and hand gestures.
