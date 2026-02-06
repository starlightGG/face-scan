# 🧬 Biometric Age Scanner & ID Generator

A futuristic, browser-based biometric scanner that uses 3D face mesh technology to estimate biological age and generate a high-security digital ID card.

## 🚀 Overview

This project demonstrates the power of **TensorFlow/MediaPipe** running entirely in the client-side browser. It features a gamified scanning process where the user must align their nose with an orbiting target to capture volumetric face data.

Once the scan is complete, the system calculates a "Biological Age" based on cranial ratios and generates a downloadable, high-resolution **Biometric ID Card**.

## ✨ Key Features

* **Real-Time 3D Mesh:** Uses `MediaPipe Face Landmarker` to track 478 facial points at 60+ FPS.
* **Ghost Mode:** A background "skeleton" mesh that tracks expressions and head movements in real-time behind the UI.
* **Gamified Scanning:** Users must follow an orbiting target to ensure a full frontal and semi-profile capture.
* **Precision Lock:** Visual feedback ring that highlights the nose tip and locks onto the target when aligned.
* **Canvas ID Generation:** Automatically generates a `.png` ID card with the user's photo, verified age, and a unique cryptographic hash.
* **Privacy First:** All processing happens locally in the browser. No video data is sent to any server.

## 🛠️ Tech Stack

* **HTML5 / CSS3:** Futuristic "Cyberpunk" UI design with neon aesthetics.
* **JavaScript (ES6+):** Modular architecture.
* **Google MediaPipe:** Machine Learning for face landmark detection.
* **HTML5 Canvas:** For real-time drawing of the mesh, target ring, and ID card generation.

## 📦 How to Run

Host it to github pages OR any static pages demo is located [here](https://starlightgg.github.io/face-scan).

### Option 1: VS Code (Recommended)
1.  Open the project folder in **VS Code**.
2.  Install the **"Live Server"** extension.
3.  Right-click `index.html` and select **"Open with Live Server"**.

### Option 2: Python
If you have Python installed, open your terminal in the project folder and run:
```bash
python -m http.server 8000
