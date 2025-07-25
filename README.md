# ParkingSpace-Counter
## Overview

This Python project utilizes the OpenCV library to detect and count the number of available parking spaces in a given parking lot or area. The system uses computer vision techniques to analyze live or recorded video footage from a camera placed in the parking area and identifies whether each parking space is occupied or vacant.

## Features

- Real-time parking space detection: The system processes video input in real-time and provides instant updates on parking space availability.
- Occupied/vacant status: Each parking space is marked as either occupied or vacant.
- Counting functionality: The system keeps track of the total number of available parking spaces as well as the number of occupied spaces.

## Dependencies

To run this project, you need to have the following dependencies installed:

- Python 3.x
- OpenCV (cv2) library
- Optionally, a webcam or video feed as input source

You can install the required Python packages using pip:

```bash
pip install opencv-python 
```

## How it Works

1. **Input Video Feed**: The system takes a video feed from a camera, either live or recorded.
2. **Preprocessing**: The video frames are preprocessed to enhance the features necessary for parking space detection. This may include color filtering, noise reduction, and resizing.
3. **Object Detection**: The OpenCV library is used to perform object detection on each frame. Specifically, the system identifies vehicles in the parking lot.
4. **Parking Space Detection**: The system determines parking space occupancy by analyzing the position of vehicles within each parking space. If a vehicle is detected within the boundaries of a parking space, that space is marked as occupied; otherwise, it's marked as vacant.
5. **Counting**: The system keeps track of the total number of parking spaces and the number of occupied spaces. It updates these counts in real-time.
6. **Display or Output**: The project can display the parking lot layout with each parking space's status (occupied/vacant) through a GUI or output this information to a file or console.

