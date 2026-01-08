🧙‍♂️ Real-Time Invisible Cloak using OpenCV

A Harry Potter–inspired computer vision project that creates a real-time invisibility effect by detecting a specific color (red cloak) and replacing it with a previously captured background using Python and OpenCV.

This project demonstrates core computer vision concepts such as color space conversion, masking, morphological operations, and real-time video processing.

📌 Project Overview

The Invisible Cloak effect works by:

Capturing a clean background frame.

Detecting a red-colored cloak in the live video stream.

Replacing the detected cloak region with the background pixels.

Producing a real-time invisibility illusion.

🎯 Features

🎥 Real-time video processing

🎨 Color-based object segmentation (HSV)

🧹 Noise removal using morphological operations

🪄 Background replacement for invisibility effect

⚡ Lightweight & fast (no deep learning required)

🛠️ Tech Stack

Programming Language: Python

Libraries: OpenCV, NumPy

Concepts Used:

Computer Vision

Color Space Transformation (BGR → HSV)

Masking & Bitwise Operations

Morphological Image Processing

Real-Time Video Streaming

🔍 How It Works
1️⃣ Background Capture

A few initial frames are captured without the user present.
This static background is stored for later replacement.

2️⃣ Color Detection (HSV)

The live frame is converted from BGR to HSV color space.
Red color is detected using two HSV ranges (since red wraps around the hue spectrum).

3️⃣ Mask Creation

A binary mask is generated where:

White pixels → cloak region

Black pixels → rest of the frame

Noise is removed using erosion and dilation.

4️⃣ Invisibility Effect

The cloak region is replaced with background pixels.

Remaining areas show the live video feed.
