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

While training I realized that replicating posing routines is extremely difficult.  
Unlike standard lifts, poses require **precise control, symmetry, and tempo**, but athletes often lack objective feedback.  

This project explores how computer vision can provide:
- Real-time angle detection (to compare left vs right side poses).  
- Tempo tracking (to slow down transitions and hold poses correctly).  
- Range of motion analysis (ensuring consistent posture between rounds).  

The long-term goal is to help athletes practice posing with the same kind of feedback we already use for strength training.

