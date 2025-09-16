Video Rep & Tempo Analyzer

A Python tool that uses pose estimation to analyze strength training reps from webcam or video.
It detects joints, counts reps, measures range of motion (ROM) and tempo, and provides clear feedback such as:

“Hit full ROM”

“Slow the eccentric”

“Watch torso sway”

Features

Detect body landmarks with MediaPipe

Count reps for common lifts (squats, curls, lateral raises, RDLs)

Compute joint angles (elbow, shoulder, hip, knee) per frame

Calculate ROM and tempo for each rep

Export session metrics to CSV/PDF

Overlay feedback directly on video

Tech Stack

Python

OpenCV - video input/output

MediaPipe - pose estimation

NumPy / Pandas - metrics & analysis

Matplotlib / ReportLab - visualization & reports

Motivation

Training without feedback makes it difficult to control tempo or maintain consistent form.
This project explores how computer vision can provide:

Real-time angle detection for symmetry and posture

Range of motion analysis for consistent movement quality

The goal is to deliver actionable feedback that helps athletes train more effectively.


ai-workout/
├── datasets/
│   ├── raw/
│   ├── keypoints/
│   └── README.md
├── notebooks/
│   └── keypoint_extraction.ipynb
├── src/
│   └── extract_keypoints.py
├── .gitignore
├── README.md
└── LICENSE

