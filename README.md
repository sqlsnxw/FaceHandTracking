# FaceHandTracking

A little computer-vision project that lets you control your mouse with your hand and
tracks your face through the webcam. Built with OpenCV and MediaPipe.

## What it does

- Move the cursor by moving your open palm around
- Make an ASL "A" sign (basically a fist) to left click
- Detects your face and draws the landmarks on it

## Running it

You'll need Python and a webcam.

```
pip install -r requirements.txt
pip install pynput
```

Then run:

```
python "import cv2.py"
```

A window opens with your camera feed and the tracking drawn on top. Move your palm to
move the mouse, fist to click. Close the window to quit.

It works best with good lighting. This is a hobby project, so the gesture detection isn't
perfect. If it feels off you can tweak the confidence values near the top of the script.
