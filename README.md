# Task 1 – Visualize CNN Activation Maps (Emotion Detection)

This task demonstrates how to visualize **activation maps** of a convolutional neural network (CNN) trained for facial emotion detection. Activation maps help us understand which parts of an image influence specific filters in the network.

---

## 📌 Objective

- Visualize intermediate feature maps from convolutional layers.
- Use a pre-trained CNN model for facial emotion detection.
- Gain interpretability into how CNNs learn and detect emotion.

---

## 🧠 Model Details

- Model architecture loaded from `model_a1.json`
- Weights loaded from `model_weights1.h5`
- Input shape: `(48, 48, 1)` grayscale facial image
- Output: 7 emotion classes (e.g., happy, sad, angry, etc.)

---

## 🧪 Features

- Visualizes activations from convolutional and ReLU layers.
- Automatically skips non-convolutional layers (like dense/flatten).
- Saves activation maps as `.png` images in timestamped folders.

---

## 🚀 How to Run

1. **Install dependencies** using:

pip install -r requirements.txt

Launch the notebook in VS Code or Jupyter:
jupyter notebook activation_maps.ipynb
Place your test image (48x48 grayscale face) inside a folder (e.g., test/) and update the image path in the notebook:
image_path = "test/happy/im3.png"
Run all cells to:

Load the model

Preprocess the image

Visualize and save activation maps

## 🧾 Requirements
tensorflow
numpy
opencv-python
matplotlib

## 📈 Output
Image grids showing which filters activate for each layer.
Results saved automatically in activation_outputs/run_<timestamp>/.

## 📌 Note
Make sure your test image is a 48x48 grayscale face image.
If the image path is incorrect or unreadable, the notebook will raise an OpenCV error.

## ✅ Task Completed For
NullClass Internship – June–July 2025
By: Aryan Jha