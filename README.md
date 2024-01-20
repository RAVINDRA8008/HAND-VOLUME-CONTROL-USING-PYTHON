# HAND-VOLUME-CONTROL-USING-PYTHON
This Python script utilizes the mediapipe library to perform hand tracking and control system volume based on hand gestures. The script uses the cv2 (OpenCV) library for image processing, pyautogui for controlling system volume, and mediapipe for hand tracking.

## Setup and Dependencies
Before running the script, make sure to install the required libraries. You can install them using the following commands:

```
pip install mediapipe
pip install opencv-python
pip install pyautogui
```

## Usage
1) Run the script in a Python environment:
```
python hand_volume_control.py
```
2) The script will access your webcam and display the camera feed.

3) Use your hand to control the volume:
   Stretch your thumb and index finger to increase volume.
   Bring your thumb and index finger together to decrease volume.
4) Press the 'Esc' key to exit the script.

   
## Code Explanation
The script does the following:

1) Captures video frames from the webcam using OpenCV.
2) Uses mediapipe to detect and track hand landmarks.
3) Draws landmarks on the video feed.
4) Calculates the distance between two specific landmarks (thumb and index finger).
5) Adjusts system volume based on the distance:
If the distance is greater than 40, it increases the volume.
If the distance is less than or equal to 40, it decreases the volume.


## Libraries Used
1) cv2 (OpenCV): Used for capturing and processing webcam frames.
2) mediapipe: Provides hand tracking functionalities.
3) pyautogui: Used for controlling system volume.

## Notes
Make sure your webcam is properly connected and accessible.
Adjust the volumeup and volumedown keys in the pyautogui.press() function based on your system's configuration.
