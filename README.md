
# Parking Space Occupancy Detector

This Python script is designed to detect the occupancy of parking spaces in a given video feed. It uses computer vision techniques to analyze each frame of the video and determine whether parking spaces are occupied or vacant.

## Features

- **Parking Space Detection:** The script identifies parking spaces within the provided video feed and monitors them for occupancy.
- **Real-Time Updates:** It provides real-time updates on the number of vacant and occupied parking spaces.
- **Visualization:** Occupancy status is visually represented with bounding boxes around parking spaces and occupancy counts displayed on the image.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- `cvzone` library

## Usage

1. Ensure that you have Python installed on your system.
2. Install the required dependencies using `pip install opencv-python numpy cvzone`.
3. Clone the repository or download the script.
4. Run the script using `python main.py`.
5. Press 'q' to exit the script.

## Instructions for Use

### Step 1: Parking Space Positioning

Before running the main script, it's necessary to obtain the positions of parking spaces within the parking lot. This is done by running the provided `parking_picker.py` script.

python parking_picker.py


This script allows you to select parking spaces by clicking on the image. Left-click to mark a parking space and right-click to remove a previously marked one. Once you're satisfied with the selected positions, close the window.

### Step 2: Running the Main Script

After obtaining the parking space positions, you can run the main script `main.py` to start monitoring parking space occupancy.


python main.py


The script will open the video feed and display the occupancy status of each parking space in real-time. Press 'q' to exit the script.

## Note

- Make sure to place the video file named `carPark.mp4` in the same directory as the script.
- The parking space positions are saved to a file named `CarParkPos` in the same directory.

