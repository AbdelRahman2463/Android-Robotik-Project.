# Android Robotik Project

This is an Android application designed to control a robot, featuring Bluetooth connectivity, joystick control, and camera-based line and ball following capabilities.

## Features

*   **Bluetooth Connectivity:** Connects to a robot via Bluetooth.
*   **Joystick Control:** Manual control of the robot using an on-screen joystick.
*   **Camera Integration:** Utilizes CameraX for real-time video preview.
*   **Line Following:** Autonomous mode to follow a line using camera vision.
*   **Ball Following:** Autonomous mode to follow a ball using camera vision.
*   **Battery Monitoring:** Displays the robot's battery voltage.

## Setup and Installation

1.  Clone the repository:
    ```bash
    git clone [repository_url]
    ```
2.  Open the project in Android Studio.
3.  Build and run the application on an Android device.

## Permissions

The application requires the following permissions:

*   `android.permission.CAMERA`
*   `android.permission.BLUETOOTH_CONNECT` (Android 12+)
*   `android.permission.BLUETOOTH_SCAN` (Android 12+)

## Usage

1.  **Connect to Robot:** Tap the "Connect" button to establish a Bluetooth connection with your robot.
2.  **Manual Control:** Use the on-screen joystick to control the robot's movement. Adjust speed with the slider.
3.  **Camera Modes:**
    *   Tap "Toggle Camera" to start the camera preview.
    *   Select "Start Line" or "Start Ball" to activate autonomous line or ball following modes.
4.  **Battery Check:** Tap "Get Battery" to view the robot's battery level.

## Contributing

Feel free to fork this repository and contribute. Please open an issue or pull request for any changes.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
