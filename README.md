# 🖱️ AIR MOUSE: AI-Powered Virtual Controller

A high-performance virtual mouse system that enables OS-level control through real-time hand gesture recognition. Built with Python and MediaPipe, this project maps 21 digital hand landmarks to screen coordinates for a "touchless" interface experience.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-007fba?style=for-the-badge&logo=google-chrome&logoColor=white)

---

## 🚀 Key Features
- **Precise Navigation:** Real-time cursor tracking using the Index Finger Tip.
- **Gesture-Based Interaction:** - **Left Click:** Index + Thumb pinch.
  - **Right Click:** Middle + Thumb pinch.
  - **Smooth Scrolling:** Move hand vertically with the Ring Finger extended.
- **Visual Debugger:** Integrated red skeleton and white landmark overlay.
- **Jitter Reduction:** Implemented linear interpolation smoothing for stable cursor movement.

## 🛠️ Technical Stack
- **Python 3.11**
- **MediaPipe 0.10.14** (Landmark extraction)
- **PyAutoGUI** (OS Automation)
- **OpenCV 4.10.0.84** (Frame processing)
- **NumPy 1.26.4** (Coordinate mapping)

## 📦 Installation
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/Jemelimercy/Air-Mouse-Pro.git](https://github.com/Jemelimercy/Air-Mouse-Pro.git)
   cd AIR-MOUSE

2. Install dependencies:
    pip install -r requirements.txt

3. Run the engine:
   python main.py

🧠 Logic & Mathematics
    The system utilizes Euclidean Distance to trigger clicks: 

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$


When the distance between the Thumb (ID 4) and Index (ID 8) falls below a specific pixel threshold, a pyautogui.click() event is dispatched.

Developed as an exploration into Human-Computer Interaction (HCI).


