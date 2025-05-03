# American Sign Language Translator 🤟🧠

A real-time American Sign Language (ASL) translator desktop application built using Python, OpenCV, MediaPipe, TensorFlow (MobileNet), and Tkinter.

## 🔍 Overview

This application uses your webcam to detect hand gestures representing ASL alphabets. It processes hand landmarks using MediaPipe, feeds the cropped hand image to a pre-trained MobileNet model for prediction, and displays the translated letter in a GUI. It also supports speech output to read the formed word aloud.

## ✨ Features

- 🖐 Real-time ASL hand gesture detection
- 🧠 MobileNet-based pre-trained model for letter prediction
- 📸 Integrated webcam video feed using OpenCV
- 🖼 Tkinter-based GUI with dynamic updates
- 🔊 Converts recognized letters into spoken words using pyttsx3
- ♻️ Reset, Clear, and Exit controls for easy interaction

## 📁 Tech Stack

- **Language:** Python
- **Libraries:** OpenCV, MediaPipe, NumPy, TensorFlow, Tkinter, pyttsx3, Pillow
- **Model:** Pre-trained MobileNet-based image classifier (`.h5` format)

## 🚀 How It Works

1. Capture video from webcam.
2. Detect hand using MediaPipe and crop the region.
3. Resize the hand image to 128x128 and normalize.
4. Predict the ASL letter using the MobileNet model.
5. Show the predicted letter and append to a forming word.
6. Optional: Speak the word aloud.

## 🧠 Model

- Pre-trained MobileNet model trained to classify limited ASL alphabet letters (e.g., A, B, C, D, E, F, L).
- Input shape: 128x128 RGB images
- Model file: `trained_model.h5`
