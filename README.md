# 🖐️ FaceHandTracking

Control your computer with your hands and track your face in real time, using a
regular webcam. Built with [OpenCV](https://opencv.org/) and Google
[MediaPipe](https://developers.google.com/mediapipe).

## ✨ Features

- **Move the mouse with your palm** — hold up your open palm and the cursor follows it.
- **Left click with a gesture** — make the ASL **"A"** sign (closed fist, thumb to the side) to click.
- **Real-time face tracking** — detects your face and draws facial landmarks live.

## 📦 Requirements

- Python 3.9+
- A webcam
- Python packages:
  - `mediapipe`
  - `opencv-python`
  - `pynput` (used to control the mouse)

## 🚀 Installation

```bash
git clone https://github.com/sqlsnxw/FaceHandTracking.git
cd FaceHandTracking
pip install -r requirements.txt
# pynput is also required for mouse control:
pip install pynput
```

The hand/face model files (`hand_landmarker.task`, `face_landmarker.task`) are
included in the repo and loaded automatically at startup.

## ▶️ Usage

```bash
python "import cv2.py"
```

A window opens showing your webcam with hand and face landmarks drawn on top.
Use your palm to move the cursor and the ASL "A" gesture to click. Press the
window's close button (or `Ctrl+C` in the terminal) to quit.

## 🎮 Gesture reference

| Gesture | Action |
|---------|--------|
| Open palm | Move the mouse cursor |
| ASL "A" (closed fist) | Left click |
| Face in frame | Tracked with landmarks drawn |

## 📝 Notes

- Good, even lighting improves tracking accuracy.
- This is a personal/educational project — gesture detection is best-effort and
  may need tuning of the confidence thresholds in the script.
