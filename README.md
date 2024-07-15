
## Intel Vehicle Cut-In Detection

Solution developed as a submission for Intel Unnati Industrial Training Program 2024.

This repository contains code for detecting vehicle cut-in events using computer vision techniques. The project utilizes the YOLOv8 model for object detection and calculates various metrics to identify potential cut-in scenarios.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Technical Approach](#technical-approach)
- [License](#license)

## Introduction

Vehicle cut-in detection is crucial for Advanced Driver Assistance Systems (ADAS) and autonomous driving. This project aims to detect cut-in events by analyzing video frames from a car's camera. The system identifies vehicles and their positions, calculates relevant metrics, and issues warnings if a vehicle cuts in within critical thresholds.

## Installation

To get started with this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/achalbajpai/vehicle-cut-in/tree/main/Code
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Ensure you have the necessary input video file in the correct directory.
2. Run the main script:
   ```bash
   python main.py
   ```

## Technical Approach

### Object Detection Using YOLOv8

The YOLOv8 model is used for detecting vehicles and other objects in the video frames. The project utilizes the `ultralytics` library for YOLO implementation.

### Distance and Position Calculations

The code calculates various metrics for detected vehicles, including:
- Distance from the camera
- Lateral position
- Time to collision (TTC)

### Cut-In Detection

A cut-in event is detected based on the calculated metrics and predefined thresholds. The system issues warnings when potential cut-in scenarios are identified.

### Visualization

The code includes functionality to visualize the detection results, including bounding boxes, distance information, and warnings on the video frames.

## License

This project is open-source. Please refer to the repository for any specific license information.

