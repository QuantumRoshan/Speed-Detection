# Speed-Dection-System
 Real-time vehicle speed detection using OpenCV and Python, featuring object detection and tracking with speed estimation.
# Vehicle Speed Detection using OpenCV and Python

This project demonstrates real-time vehicle speed detection using OpenCV and Python. It involves detecting cars in a video feed, tracking their movements, and estimating their speeds.

## Features
- **Object Detection**: Utilizes a pre-trained Haar Cascade classifier to detect vehicles in video frames.
- **Object Tracking**: Employs dlib's correlation tracker to follow detected vehicles across frames.
- **Speed Calculation**: Estimates the speed of tracked vehicles based on their movement between frames.
- **Real-Time Processing**: Continuously processes each frame and updates vehicle information and speed.
- **Output**: Displays and saves the annotated video with detected vehicles and their speeds.

## Requirements
- Python 3.x
- OpenCV
- dlib

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/vehicle-speed-detection.git
    ```
2. Navigate to the project directory:
    ```sh
    cd vehicle-speed-detection
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. Ensure the correct paths are set for the classifier file and the video file in the script.
2. Run the script:
    ```sh
    python vehicle_speed_detection.py
    ```
3. The processed video with speed annotations will be displayed and saved as `outTraffic.avi`.

## Code Overview
- `estimateSpeed(location1, location2)`: Calculates the speed of a moving vehicle between two points.
- `trackMultipleObjects()`: Main function to track and estimate the speed of multiple vehicles.
  - Initializes various variables for tracking cars and their speeds.
  - Processes each video frame, updates trackers, detects new cars, and calculates speeds.
  - Displays and saves the output video with detected vehicles and their speeds.

## Acknowledgments
This project is inspired by various resources and tutorials available on vehicle detection and tracking using OpenCV and dlib.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
