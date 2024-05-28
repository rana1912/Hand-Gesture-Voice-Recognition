# Hand-Gesture-Voice-Recognition
This project implements a real-time hand gesture recognition system using OpenCV. It captures video from a webcam, processes frames to isolate the hand, and detects the number of fingers using convex hull and convexity defects. The system provides visual feedback and triggers actions based on detected gestures.
# Hand Gesture Recognition System

This project implements a real-time hand gesture recognition system using OpenCV and computer vision techniques. It captures video from a webcam, processes the frames to isolate the hand, and detects the number of fingers using convex hull and convexity defects. The system provides visual feedback and triggers actions based on the detected gestures.

## Features
- Real-time video capture and processing.
- Background subtraction to isolate the hand.
- Convex hull and convexity defects analysis to detect fingers.
- Adjustable parameters through trackbars.
- Visual feedback with contours and convex hull drawn on the video feed.
- Trigger actions based on the number of detected fingers.

## Usage
1. Run the main script to start the gesture recognition system:
    ```bash
    python main.py
    ```

2. Use the trackbars to adjust the `threshold` value in real-time.

## Project Description
The hand gesture recognition system utilizes OpenCV to process video frames from a webcam. The main steps include background subtraction to isolate the hand, converting the image to grayscale, applying Gaussian blur, and thresholding to segment the hand region. The system then uses convex hull and convexity defects analysis to detect the number of fingers extended. Based on the detected gestures, predefined actions are triggered. The system also includes a user interface with trackbars to adjust parameters in real-time.

## Parameters
- `cap_region_x_begin`: Starting x-coordinate (50% from the left) for the capture region.
- `cap_region_y_end`: Ending y-coordinate (80% from the top) for the capture region.
- `threshold`: Binary threshold for image segmentation.
- `blurValue`: Gaussian blur parameter to smooth the image.
- `bgSubThreshold`: Background subtraction threshold.
- `learningRate`: Learning rate for background subtraction model.

