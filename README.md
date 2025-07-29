# PushUp-and-Plank-Counter

# Push-Up Counter & Plank Timer using Python (OpenCV + Mediapipe)

##  Project Overview

This Python project uses your **device camera** to:

* **Count push-ups automatically** by detecting your elbow angles.
* **Measure plank hold time** using body alignment detection.
* Show **live count and timer** on your webcam feed for motivation.

It is beginner-friendly and practical for **portfolio, GitHub, and LinkedIn**.

---

## Requirements

* Python 3.8+
* VS Code / Jupyter / Any IDE

### Install dependencies:

```bash
pip install opencv-python mediapipe numpy
```

---

##  How to Run

1️⃣ Save the provided `.py` or `.ipynb` file in your project folder.

2️⃣ Run using VS Code terminal or:

```bash
python pushup_plank_counter.py
```

3️⃣ Your webcam will open. **Ensure your camera is at chest height for best results.**

4️⃣ Press **'q'** to quit anytime.

---

##  How It Works

### Push-Up Counter:

✅ Uses **Mediapipe Pose** to track your **shoulder, elbow, wrist landmarks**.
✅ Calculates **elbow angles**:

* If **angle < 70°**: you are down.
* If **angle > 160° after down**: push-up counted.

### Plank Timer:

✅ Checks **vertical alignment** of shoulder, hip, and ankle.
✅ If aligned within thresholds:

* Timer starts.
  ✅ If posture breaks:
* Timer resets.

---

## User Manual

✅ **For Push-Ups:**

* Position camera so your **upper body is visible clearly**.
* Do full push-ups (lock elbows fully at top).
* Ensure lighting is good.

✅ **For Plank:**

* Face sideways to the camera.
* Keep your body in a straight line.
* Avoid head tilts for consistent detection.

✅ Press **'q' to exit safely**.

---

## Output

* Displays live **push-up count**.
* Displays **plank timer (seconds held)**.
* Shows body landmarks for learning.


