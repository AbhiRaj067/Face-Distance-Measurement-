# Face Distance Measurement

_Developed during my internship at GB Softronics Solution_

## Overview

This project implements a system to measure the distance from a person's face to the camera in real time using computer vision and Python. The solution combines mathematical principles and image processing techniques to deliver accurate estimations, with robust detection and practical visualization.

## Key Features

- **Face Detection:**  
  Uses OpenCV's pre-trained Haar cascades or Dlib/cvzone FaceMesh models for precise face localization, with reliability across varied lighting conditions and angles.

- **Distance Calculation:**  
  Estimates real-world distance utilizing the principle of similar triangles. Measures the pixel width of the detected face and compares it to a known reference width, calculating distance with the formula:  

Distance
=
(
Known Width
×
Focal Length
)
/
Face Width in Image
Distance=(Known Width×Focal Length)/Face Width in Image
The focal length is determined through a calibration process with a known face size at a fixed distance.

- **Real-Time Processing:**  
Streams and processes webcam video frames on-the-fly to detect faces and overlay distance measurement instantly.

- **Output Visualization:**  
Displays the distance annotation and project details directly on the live video feed using OpenCV and cvzone drawing tools for clarity and impact.

## Challenges and Solutions

- **Camera Calibration:**  
Adjusted for different webcams to achieve correct focal length and accurate results.
- **Lighting Variations:**  
Fine-tuned detection algorithms to function reliably in low-light and high-glare environments.
- **Accuracy Enhancements:**  
Smoothed output by averaging over multiple frames and managed edge cases (e.g., partial faces).

## Outcome

The project delivers reliable, real-time distance measurements, with promising applications in:
- Interactive systems and user experience enhancement
- Social distancing monitoring
- AR/VR and gesture input

This work deepened my understanding of computer vision, real-time video processing, and the effective application of mathematical models to solve real-world problems.

## Technologies Used

- Python 3
- OpenCV
- Dlib or cvzone (FaceMeshModule)
- numpy

## Setup & Usage

1. **Install dependencies:**

2. **Run the script:**

Ensure your webcam is connected and accessible.

## Example Output

Live webcam feed displaying:
- Detected face(s) with bounding boxes or landmarks
- Real-time distance annotation in centimeters
- Dynamic project credentials beside the video frame

## Author

**Abhishek Raj**  
Intern, GB Softronics Solution  
Employee ID: GBSOFT-INT175

---

For feedback, suggestions, or collaboration, please open a GitHub issue or contact via profile.







