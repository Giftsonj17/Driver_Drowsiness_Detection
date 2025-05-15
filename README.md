"Detection of Driver Fatigue with Advanced Spatial–AI Models"
This project presents a real-time AI-based Driver Drowsiness Detection System built using YOLOv8 and computer vision techniques. It aims to enhance road safety by identifying signs of driver fatigue such as eye closure, yawning, and abnormal head movement via webcam input.

## 🚗 Project Overview

Drowsy driving contributes significantly to road accidents. Our system continuously monitors the driver’s facial behavior and triggers alerts when signs of fatigue are detected. It is lightweight, real-time, and deployable on personal computers or embedded devices (e.g., Raspberry Pi).

## 🧠 Technologies Used

- Python
- OpenCV
- YOLOv8 (Ultralytics)
- PyTorch
- Pygame
- pyttsx3 (Text-to-Speech)
- NumPy

## 📁 Dataset

- **Driver Drowsiness Dataset** – Video-based data (from IEEE)
- **YawnDD Dataset** – Image-based yawning samples (from Kaggle)

Data includes various samples of eye closure, yawning, and head movement under different lighting conditions. Preprocessing steps included:
- Frame extraction
- Resizing (224x224)
- Normalization
- Data augmentation
- Manual labeling (Drowsy / Non-Drowsy)

## 🛠️ System Architecture

- **Input Layer:** Captures live video from webcam
- **YOLOv8 Model:** Detects facial cues in real time
- **Detection Layer:** Classifies driver as Drowsy or Non-Drowsy
- **Alert System:** Audio alarms, text-to-speech messages, and logging
- **Optional:** GPS tracking and SMS alerts via Twilio (commented for privacy)

## 📈 Model Performance

- **Accuracy:** 95.3%
- **Precision:** 94.8%
- **Recall:** 96.1%
- **F1-Score:** 95.4%

## 🔊 Alerts and Features

- 🔴 Red flash overlay for drowsiness
- 🔉 Voice alerts using `pyttsx3`
- 📢 Sound alarms using `pygame`
- 📋 Logs every detected event with a timestamp

## 🖥️ How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/YourUsername/driver-drowsiness-detection.git
   cd driver-drowsiness-detection


Install required packages:
pip install -r requirements.txt

Make sure the following files are in the same directory:
drowsiness_detection.py
best.pt (YOLOv8 model weights)
Alarm audio files:

drowsy_alarm.mp3

yawn_alarm.mp3

head_movement_alarm.mp3

Run the script:
python drowsiness_detection.py


👥Authors
Joel Giftson J – Saranathan College of Engineering

Seenivasa Perumal N

Sudharsan K

Project Guide: Mr. Arunprakash (Assistant Professor)

📜 Conference
Presented at the 7th International Conference on Artificial Intelligence, Data Science & Cyber Security, Indra Ganesan College of Engineering, 2025.

🔗 Links
Project Presentation Slides

Live Demo / Video (optional)

Paper / Certificate



