Video Rep & Tempo Analyzer

A Python tool that uses pose estimation to analyze strength training reps from webcam or video.  
The system detects joints, counts reps, measures range of motion (ROM) and tempo, and gives coaching feedback like:

- “Hit full ROM”  
- “Slow the eccentric”  
- “Watch torso sway”  

Why? Because tempo control + ROM are strong proxies for **mind-muscle connection** and effective training.


## MVP
- Detect body landmarks using [MediaPipe](https://developers.google.com/mediapipe).  
- Count reps for common lifts (squats, curls, lateral raises, RDLs).  
- Compute elbow/shoulder/hip/knee angles per frame.  
- Calculate ROM & tempo for each rep.  
- Export per-set metrics to **CSV/PDF**.  
- Overlay feedback directly on video.

---

## Tech Stack
- **Python**  
- **OpenCV** → video input/output  
- **MediaPipe** → pose landmarks  
- **NumPy / Pandas** → metrics & analysis  
- **Matplotlib / ReportLab** → visualization & reports

 ## Motivation

While training, I noticed that replicating certain exercises and posing routines can be challenging without feedback.

This project explores how computer vision can help by providing:

Real-time angle detection to compare left and right side movements.

Range of motion analysis to ensure consistent posture and form.

The long-term goal is to give athletes actionable feedback that supports better training and performance.

