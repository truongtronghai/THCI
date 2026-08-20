### Touchless Human-Computer Interaction (HCI) System

A lightweight, open-source gesture control system that translates real-time hand movements into OS-level mouse inputs using a standard webcam. No specialized depth hardware (like Leap Motion or Kinect) is required. 

### 🚀 Overview

This project leverages computer vision and machine learning to create a touchless user interface. By tracking 21 distinct hand landmarks, the system allows users to navigate their operating system, move the cursor, and execute clicks entirely through mid-air hand gestures. 

### 🛠️ Tech Stack

* **OpenCV:** Handles video capture, frame transformation (mirroring), and visual feedback rendering.
* **Google MediaPipe:** Runs the pipeline to detect and extract 3D hand joint coordinates.
* **PyAutoGUI:** Translates mathematical coordinates into hardware-level OS mouse actions.

### 🌟 Key Features

* **Zero-Hardware Dependency:** Works flawlessly on any standard 2D webcam.
* **Mirrored Intuitive Control:** Automatically flips the camera feed to match natural hand movements.
* **Dynamic Click Trigger:** Uses a precise distance algorithm between the index finger and thumb to simulate a physical mouse click.

### 🔧 Installation & Setup

1. **Clone the repository:**

bash

git clone https://github.com/yourusername/touchless-hci.git
cd touchless-hci

Use code with caution.

1. **Install the dependencies:**

bash

pip install opencv-python mediapipe pyautogui

Use code with caution.

1. **Run the application:**

bash

python gesture_mouse.py

Use code with caution.

### 🎮 How to Use

* **Move Cursor:** Raise your hand and move your index finger. The cursor will follow your finger tip across the screen.
* **Left Click:** Pinch your thumb and index finger closely together and release.
* **Exit Program:** Press the q key on your keyboard while focusing on the webcam window to safely close the application.