# Eye-Controlled Mouse using MediaPipe

## Overview
This project enables controlling your mouse cursor using eye movements detected via a webcam. It leverages **MediaPipe's Face Mesh** model to track eye landmarks and uses **PyAutoGUI** to move the cursor and perform mouse clicks based on blinking.

---

## Features
- Real-time eye gaze tracking to move the mouse cursor.
- Blink detection for mouse click simulation.
- Uses a simple webcam setup — no additional hardware required.
- Visual feedback by drawing landmarks on the webcam feed.

---

## Technologies Used
- Python 3.9
- OpenCV
- MediaPipe
- PyAutoGUI

---

## Installation

1. Clone the repository or download the source code.

2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Usage
Run the main program:

bash
Copy
Edit
python main.py
A window will open showing your webcam feed with eye landmarks.

Move your eyes to control the mouse cursor.

Blink to simulate a mouse click.

Press q to quit the program.

File Structure
bash
Copy
Edit
eye-controlled-mouse-mediapipe/
│
├── main.py               # Main application code
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
├── license.txt           # License information
├── flowchart.png         # (Optional) Flowchart diagram
├── architecture.png      # (Optional) System architecture diagram
└── utils/                # Utility modules (if used)
    ├── gaze_tracker.py
    └── blink_detector.py
Troubleshooting
Make sure your webcam is connected and accessible.

If you experience lag, try reducing your webcam resolution.

Ensure Python packages are correctly installed.

License
This project is licensed under the MIT License - see the license.txt file for details.

Acknowledgements
MediaPipe for face mesh detection.

PyAutoGUI for mouse control.

OpenCV for video capture and image processing.
