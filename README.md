# Hand Gesture Controlled Brightness Adjuster

This project implements a hand gesture-controlled brightness adjustment system using OpenCV, Mediapipe, and the `screen_brightness_control` library. The brightness is controlled by calculating the distance between the thumb and index finger using a webcam feed, and adjusting the screen brightness accordingly.

## Features

- Real-time hand tracking using Mediapipe's hand landmark model.
- Distance calculation between thumb and index finger to control brightness.
- Dynamic brightness adjustment between 0% and 100%.
- Uses OpenCV for video capture and drawing hand landmarks.
- Simple and responsive control using hand gestures.

## Requirements

- Python 3.x
- OpenCV
- Mediapipe
- Numpy
- Screen Brightness Control (`screen_brightness_control`)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/hand-gesture-brightness-adjuster.git
    cd hand-gesture-brightness-adjuster
    ```

2. Install the required Python libraries:

    ```bash
    pip install opencv-python mediapipe screen-brightness-control numpy
    ```

## How to Run

1. Ensure your webcam is connected and accessible.

2. Run the script:

    ```bash
    python hand_brightness_control.py
    ```

3. Place your hand in front of the camera. The software will track your hand and adjust the brightness based on the distance between your thumb and index finger.

4. Press 'q' to exit the program.

## How It Works

- The software captures video input from the webcam using OpenCV.
- Mediapipe's hand detection model processes each frame to detect hand landmarks.
- The distance between the tip of the thumb (landmark 4) and the index finger (landmark 8) is calculated using the Euclidean distance formula.
- The brightness is then mapped to this distance and adjusted using the `screen_brightness_control` library.
![image](https://github.com/user-attachments/assets/468147f0-f3fb-4467-ac1a-d217a89f5906)
![image](https://github.com/user-attachments/assets/47123dcc-0e6f-4270-b652-648657430d7d)
## Dependencies

- **OpenCV**: Used for real-time video capture and display.
- **Mediapipe**: Provides hand tracking functionality.
- **Numpy**: For efficient mathematical operations.
- **Screen Brightness Control**: Used to adjust the system's screen brightness.



