# Lane Detection Using Classical Edge Detection Methods

This project implements and compares multiple classical computer vision edge detection techniques for lane detection in road images.

It is built using OpenCV and evaluates how different edge detectors perform in real-world driving scenes.

---

## 📌 Objective

The goal is to:
- Understand how different edge detection algorithms behave
- Compare their performance on road lane detection
- Build a full image processing pipeline without deep learning

---

## 🧠 Techniques Used

The following methods are implemented and compared:

### 1. Preprocessing
- Grayscale conversion
- Gaussian Blur (noise reduction)

### 2. Edge Detection Methods
- Sobel Operator
- Scharr Operator
- Prewitt Operator
- Laplacian Operator
- Canny Edge Detector
- Simple Thresholding (baseline)

---

## 🔄 Pipeline Flow
Input Image
→ Grayscale
→ Gaussian Blur
→ Edge Detection Methods
→ Lane Visualization


---

## 📊 Key Observations

- **Canny** produces the cleanest and most stable lane boundaries
- **Scharr** improves on Sobel with better gradient accuracy
- **Prewitt** is simple but noisy
- **Laplacian** is sensitive and unstable for real road scenes
- **Thresholding** is too naive for complex environments

---

## 📁 Dataset

- Source: Kaggle preprocessed lane dataset
- Contains road driving frames and lane annotations

---

## 🛠 Tech Stack

- Python
- OpenCV
- NumPy
- Matplotlib
- KaggleHub

---

## Output

The pipeline visualizes:

Original Image
Grayscale
Gaussian Blur
Sobel Edges
Scharr Edges
Prewitt Edges
Laplacian Edges
Canny Edges
Threshold Result
