# PINKU - AI / YOLO Module

## Responsibility

This module handles the Artificial Intelligence and YOLO-based vehicle
detection component of the Vehicle Detection & Traffic Analysis project.

## Main Tasks

- Configure and load the YOLO object detection model
- Detect vehicles from images and video frames
- Identify supported vehicle categories:
  - Car
  - Motorcycle
  - Bus
  - Truck
- Generate bounding boxes around detected vehicles
- Calculate and return confidence scores
- Provide a reusable detection function for other project modules
- Provide structured detection results for integration with:
  - Video processing
  - Vehicle counting
  - UI/dashboard
  - Testing and performance analysis

## Detection Flow

```text
Input Image / Video Frame
          |
          v
      YOLO Model
          |
          v
    Object Detection
          |
          v
    Vehicle Filtering
          |
          v
+---------+----------+
|         |          |
Car   Motorcycle   Bus   Truck
          |
          v
Bounding Box + Confidence
          |
          v
Structured Detection Results