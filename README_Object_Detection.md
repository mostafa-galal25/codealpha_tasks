# Object Detection and Tracking

Using YOLOv8 + SORT Tracking Algorithm

## 📌 Overview

This project performs **real-time object detection and multi-object
tracking** using:

-   **YOLOv8** --- for object detection\
-   **SORT (Simple Online and Realtime Tracking)** --- for assigning IDs
    and tracking objects across frames\
-   **OpenCV** --- for reading video frames and visualization

The project loads a video, detects objects frame by frame, then tracks
each object with a persistent ID.

## 🚀 Features

-   Real-time object detection using YOLOv8n (fast and lightweight)
-   Tracking with Kalman filters + Hungarian matching (SORT)
-   Displays object bounding boxes + unique tracking IDs
-   Works with any video input

## 🧰 Requirements

    pip install ultralytics opencv-python numpy filterpy

## 📁 Project Structure

    Object Detection and Tracking/
    │── SORT implementation
    │   ├── linear_assignment
    │   ├── IoU matching
    │   ├── KalmanBoxTracker
    │   └── Sort class
    │── YOLO detection + video tracking loop
    └── walking_people.mp4

## ▶️ How to Run

Edit:

    cap = cv2.VideoCapture("your_video.mp4")

## 🛠 Technologies Used

-   Python
-   OpenCV
-   Ultralytics YOLOv8
-   Kalman Filter
-   Hungarian Algorithm
