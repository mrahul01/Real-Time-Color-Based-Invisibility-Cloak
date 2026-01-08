# 🧙‍♂️ Real-Time Invisible Cloak using OpenCV (Python)

A Harry Potter–inspired computer vision project that creates a real-time invisibility effect by detecting a specific color (red cloak) and replacing it with a previously captured background.

This project demonstrates core computer vision techniques such as color-space transformation, masking, morphological operations, and real-time video processing — all implemented without deep learning for efficiency and clarity.

## ✨ Features

- 🎥 Real-time webcam video processing
- 🎨 Color-based object segmentation using HSV color space
- 🧹 Noise reduction via morphological operations (erosion & dilation)
- 🪄 Background capture and pixel-level replacement for invisibility effect
- ⚡ Lightweight, fast, and easy to run (OpenCV + NumPy only)

## 🛠️ Tech Stack

**Language:** Python 3.8+

**Libraries:**
- OpenCV (cv2)
- NumPy

## 📦 Installation

1. (Optional) Create a Virtual Environment
   ```
   python -m venv venv
   source venv/bin/activate      # macOS / Linux
   venv\Scripts\activate         # Windows
   ```

2. Install Dependencies
   ```
   pip install opencv-python numpy
   ```

💡 If you are running in a headless environment (e.g., server), use:
```
pip install opencv-python-headless numpy
```

## ▶️ Usage

- Ensure your webcam is connected.
- Move out of the camera frame (or remove the cloak) for a few seconds so the system can capture a clean background.
- Run the script:
  ```
  python invisibility_cloak.py
  ```

The program will:
- Capture background frames
- Process video in real time
- Replace red-colored regions with background pixels
- Press `q` to quit.
