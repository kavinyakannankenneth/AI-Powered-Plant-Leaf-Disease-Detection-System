# AI-Powered Plant Leaf Disease Detection System

A desktop application built with Python, TensorFlow/Keras, OpenCV, and Tkinter to classify plant leaf diseases from images and provide treatment recommendations.

## Features
- **GUI Interface:** User-friendly Tkinter desktop interface for uploading training images, triggering model training, and running disease predictions.
- **Image Preprocessing:** Performs grayscale conversion, image inversion, median blurring, and Non-Local Means denoising using OpenCV and Pillow.
- **Multi-Crop Disease Classification:** Classifies 14 leaf conditions across Citrus, Rice, and Tomato crops using a pre-trained Convolutional Neural Network (`leafmodel.h5`).
- **Treatment Guidance:** Displays the predicted disease class along with recommended fungicide or agricultural management steps.

## Supported Classes (14)
- **Citrus:** Black Spot, Canker, Greening, Healthy, Melanose
- **Rice:** Bacterial Leaf Blight, Brown Spot, Leaf Smut
- **Tomato:** Bacterial Spot, Early Blight, Healthy, Late Blight, Leaf Mold, Septoria Leaf Spot

## Project Structure
- `Main.py` — Main Tkinter GUI application for image upload, preprocessing, testing, and displaying results.
- `model.py` — CNN architecture and training script used to generate `leafmodel.h5`.
- `leafmodel.h5` — Pre-trained Keras deep learning model weights.
- `*.jpg / *.JPG` — Sample leaf images included for testing predictions.

## Prerequisites & Installation
1. Clone the repository:
   ```bash
git clone https://github.com/kavinyakannankenneth/AI-Powered-Plant-Leaf-Disease-Detection-System.git
   cd AI-Powered-Plant-Leaf-Disease-Detection-System
