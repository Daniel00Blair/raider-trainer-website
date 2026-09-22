<div align="center">
  <h1>Raider Trainer 🏋️‍♂️</h1>
  <p><b>Wright State University | CEG 4110/6110 Term Project (Group 4)</b></p>
  
  [![Python](https://img.shields.io/badge/Python-3.x-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org/)
  [![OpenCV](https://img.shields.io/badge/Vision-OpenCV-5C3EE8.svg?style=flat&logo=opencv&logoColor=white)](https://opencv.org/)
  [![Website](https://img.shields.io/badge/Live-Website-026937.svg?style=flat)](https://deepikaJirel.github.io/RaiderTrainer/)
</div>

---

> Raider Trainer is a 100% Python full-stack desktop application that tracks upper-body workouts in real-time, enforces correct form thresholds, and monitors strength training progress using deep learning and computer vision.

🔗 **[View the Live Project Website & Demos](https://deepikaJirel.github.io/RaiderTrainer/)**

## ✨ Core Features

* **Real-Time Pose Tracking:** Leverages YOLOv8 keypoints to compute 2D joint angles (shoulder, elbow, wrist). Categorizes repetition form into Correct, Intermediate, and Wrong tiers for exercises like Bicep Curls and Military Presses.
* **Automated OCR Weight Scanning:** Uses Optical Character Recognition (OCR) algorithms to automatically scan and identify printed numbers on hand weights (5, 10, or 15 lbs) via the webcam.
* **Role-Based Access Control:** Secure authentication system featuring 12-character complex password requirements, a 3-attempt lockout policy, and a dedicated Admin dashboard for account recovery.
* **Adaptive Analytics:** Evaluates post-workout user feedback to suggest adjusted reps and weights, rendering daily historical progress on embedded Matplotlib charts.
* **Atomic JSON Storage:** Monolithic architecture utilizing flat JSON files (`users.json`, `workout_logs.json`) for lightweight, local data persistence without the overhead of an external SQL database.

## 🛠️ Technology Stack

* **Language:** Python 3
* **GUI Framework:** PyQt6 / PySide6
* **Computer Vision:** OpenCV (`opencv-python`)
* **Pose Estimation Engine:** Ultralytics YOLOv8 (`yolov8n-pose.pt`)
* **Data Visualization:** Matplotlib

## 🚀 Quick Start / Local Setup

```bash
# Clone the repository
git clone [https://github.com/deepikaJirel/RaiderTrainer.git](https://github.com/deepikaJirel/RaiderTrainer.git)

# Navigate into the project directory
cd RaiderTrainer

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # Use `venv\Scripts\activate` on Windows

# Install required dependencies
pip install -r requirements.txt

# Launch the desktop application
python main.py
