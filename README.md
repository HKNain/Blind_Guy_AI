# 👁️‍🗨️ BlindVision AI

An AI-powered assistive system for the visually impaired that uses voice input/output to help users **identify objects indoors** and **navigate safely outdoors** using real-time computer vision.

---

## 🔍 Problem Statement

Visually impaired individuals face significant challenges navigating unfamiliar indoor and outdoor environments. Traditional aids like canes and guide dogs offer limited feedback and awareness. There's a need for an accessible, intelligent system that can:

- Identify objects in indoor spaces.
- Assist in avoiding obstacles outdoors.
- Operate hands-free with voice-based interaction.

**BlindVision AI** bridges this gap with a real-time, voice-controlled assistant that enables greater independence and situational awareness.

---

## 💡 Project Overview

BlindVision AI is a **Python-based assistive system** that listens to user commands, processes the environment via camera, and responds with audio feedback. It has two primary modes:

1. **Indoor Mode** 🏠  
   - Takes voice commands to find and locate specific objects.
   - Uses YOLOv8n object detection for real-time recognition.

2. **Outdoor Mode** 🚶‍♂️  
   - Continuously scans for obstacles (like poles, vehicles, etc.).
   - Alerts the user with audio warnings for safe navigation.

---

## 🛠️ Tech Stack

| Component | Description |
|----------|-------------|
| 🐍 Python | Core programming language |
| 🧠 [Ultralytics YOLOv8n](https://github.com/ultralytics/ultralytics) | Real-time object detection |
| 🎙️ Google Speech Recognition | Converts voice commands to text |
| 🔊 Google Text-to-Speech (gTTS) | Converts text responses to speech |
| 📷 OpenCV | Captures and processes video frames |
| 🔁 PyTorch | Deep learning model runtime |
| 🎧 playsound / pyttsx3 | Voice feedback (offline option also available) |

---

## 🎯 Features

- 🎤 **Voice Commands**: Fully voice-operated interface.
- 🧭 **Two Modes**:
  - *Indoor*: Detects requested objects in the environment.
  - *Outdoor*: Alerts user of obstacles using live camera feed.
- 🔈 **Audio Feedback**: All responses are spoken aloud.
- 🔌 **Modular Design**: Easy to switch between modes and extend functionality.
- 💻 **Laptop Prototype**: Runs on standard webcam and microphone.

---

## 🧪 How It Works (Workflow)

1. **Start Application**
2. **Choose Mode via Voice**: "Indoor" or "Outdoor"
3. **Indoor Mode**:
   - User: “Find bottle”
   - Camera scans environment
   - If found, response: “Bottle detected at center-left”
4. **Outdoor Mode**:
   - Constant video feed analysis
   - Voice alert: “Obstacle ahead. Move right”
5. **Repeat until exit command**

---

## 🚀 Setup Instructions

1. **Clone this repository**
```bash
git clone https://github.com/yourusername/blindvision-ai.git
cd blindvision-ai
