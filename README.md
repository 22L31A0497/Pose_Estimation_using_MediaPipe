
## 🧍 Project 2: Pose Estimation using MediaPipe

### 🔍 Overview

The **Pose Estimation Project** tracks and analyzes **human body posture** using Google’s **BlazePose** model.
It detects **33 key body landmarks** (e.g., head, shoulders, elbows, hips, knees, ankles), allowing precise tracking of movement and posture.

---

### ⚙️ How It Works

**Stage 1 – Detection:**
The system detects the human body from the frame and crops the region of interest.

**Stage 2 – Landmark Prediction:**
A trained deep learning model predicts **33 3D landmarks** along with **visibility scores**.

The model includes **temporal smoothing**, ensuring stability even in motion-heavy video frames.

---

### 🧠 Model Features

* Detects **33 human body landmarks**
* Works on both **images and live video**
* Provides **3D coordinates** for each landmark
* Optimized for **real-time processing** on CPU

---

### 🧪 Requirements

```bash
pip install mediapipe opencv-python numpy
```

---

### ▶️ How to Run

1. Clone or download the repository.
2. Modify the script to include your image path or webcam feed.
3. Run:

   ```bash
   python PoseEstimation.py
   ```
4. Example image input:

   ```python
   img = cv2.imread("J:\\my mobile photos\\IMG20230802213734.jpg")
   ```
5. The output will display a visual overlay of **33 body landmarks**.

---

### 📥 Input

* RGB image or video feed
* Works on `.jpg`, `.png`, `.mp4`, or live webcam

### 📤 Output

* Annotated image or video with 33 landmarks
* Optional visibility and connection lines

---

### 📚 Libraries Used

* **MediaPipe** – BlazePose model for landmark prediction
* **OpenCV** – Display, image capture, and frame processing
* **NumPy** – Array and mathematical operations

---

### 🚀 Example Applications

* Fitness posture tracking
* Sports performance analysis
* Human motion and gesture analysis
* Animation and AR modeling

---

### 📸 Demo Example

```python
img = cv2.imread("J:\\my mobile photos\\IMG20230802213734.jpg")
```

Displays the human pose with 33 landmark connections.

---

### 🏁 Summary

This project demonstrates **AI-powered human pose detection** using computer vision.
It’s a strong foundation for building fitness apps, motion analytics, or gesture-based control systems.
