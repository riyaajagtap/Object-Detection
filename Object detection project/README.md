# Real-Time Object Detection using CNN (Webcam)

This project demonstrates a **real-time object classification system** using a **Convolutional Neural Network (CNN)** and a **webcam**.  
The model is trained to recognize everyday objects and predict them live from the camera feed.

---

## 📌 Project Overview

The notebook captures images from a webcam, builds a custom dataset, trains a CNN model, and performs **live object recognition**.

Objects recognized in this project:
- Earbud
- Mobile Phone
- Book
- Pen

The system displays **prediction confidence percentages** in real time on the webcam feed.

---

## 🧠 How the System Works

1. **Data Collection**
   - Uses webcam input via OpenCV.
   - Captures images inside a fixed Region of Interest (ROI).
   - Stores images for each object class separately.

2. **Data Preprocessing**
   - Crops the ROI from each image.
   - Resizes images to `96 × 96`.
   - Normalizes pixel values.

3. **Model Training**
   - Builds a CNN using Keras/TensorFlow.
   - Uses convolution, pooling, dropout, and dense layers.
   - Trains the model on the captured images.
   - Saves trained weights for reuse.

4. **Real-Time Prediction**
   - Opens webcam again.
   - Runs the trained model on live frames.
   - Displays predicted object and confidence percentage.

---

## 🛠️ Technology Stack

- **Language:** Python
- **Libraries:**
  - OpenCV
  - NumPy
  - TensorFlow / Keras
  - Matplotlib
- **Model Type:** Convolutional Neural Network (CNN)

---

## 📂 Files in Repository

```text
.
├── SD_ML_IP_6.ipynb        # Main Jupyter notebook
├── README.md              # Project documentation
└── .gitignore             # Ignored files (datasets, model weights, etc.)
