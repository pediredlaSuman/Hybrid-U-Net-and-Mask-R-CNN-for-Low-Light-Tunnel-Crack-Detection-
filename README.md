# 🚧 Hybrid U-Net and Mask R-CNN for Low-Light Tunnel Crack Detection

**Skills Used:** `Python`, `TensorFlow`, `OpenCV`, `Deep Learning`, `Image Segmentation`, `Computer Vision`

---

## 🔍 Project Overview

An automated tunnel crack detection system using a hybrid deep learning architecture combining **U-Net** and **Mask R-CNN**. Designed to detect and segment hairline, transverse, longitudinal, and disguised cracks under challenging low-light conditions using the **KICT Tunnel Crack Segmentation Dataset**.

---

## 🧠 Architecture Summary

### 🧩 Step 1: Semantic Segmentation with U-Net
- Segments low-light tunnel images to generate pixel-wise crack masks.
- Handles varying illumination and captures fine crack patterns.

### 🧩 Step 2: Instance Detection with Mask R-CNN
- Uses U-Net masks to localize individual cracks.
- Enhances segmentation with instance-level refinement.
- Backbone: ResNet-101 + FPN
- Head: DeepLabV3-style decoder with ASPP for boundary precision.

---

## 🎯 Key Results

| Metric            | Score |
|-------------------|-------|
| IoU               | 0.847 |
| Dice Coefficient  | 0.918 |
| Precision         | 0.902 |
| Recall            | 0.937 |
| F1-Score          | 0.919 |
| Inference Speed   | 24 FPS |

✅ Achieved **state-of-the-art performance** compared to YOLOv5s, Mini-U-Net, and Mixed Attention models.

---

## 🗃 Dataset and Preprocessing

- **Dataset**: KICT Tunnel Crack Segmentation Dataset (11,300+ labeled images)
- **Preprocessing**:
  - Resizing: 1024×1024 px
  - CLAHE: Enhances contrast in poor lighting
  - Gaussian Noise Removal
  - Perspective Correction
  - Normalization and tensor conversion using PyTorch transforms

---

## ⚙️ Training Configuration

- **Loss**: Mean Squared Error (MSE)
- **Optimizer**: Adam (`lr = 1e-4`)
- **Scheduler**: ReduceLROnPlateau
- **Early Stopping**: Patience = 5
- **Epochs**: 30 | **Batch Size**: 4

---

## 🧪 Crack Types Handled

| Crack Type         | Precision | Recall | F1 Score |
|--------------------|-----------|--------|----------|
| Hairline Cracks     | 0.887     | 0.921  | 0.904    |
| Transverse Cracks   | 0.914     | 0.945  | 0.929    |
| Longitudinal Cracks | 0.906     | 0.931  | 0.918    |
| Branching Cracks    | 0.901     | 0.918  | 0.909    |
| Disguised Cracks    | 0.882     | 0.910  | 0.896    |

---

## 📸 Visual Results

U-Net segmentation (left), refined with Mask R-CNN (right):

<p align="center">
  <img src="https://github.com/user-attachments/assets/70d85f88-95b0-48dc-bd72-ac4caa48de5a" width="600"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/68d5ba4a-0c28-4916-baa9-770f382fe2ad" width="500"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f964c49d-d0f3-49f9-a924-9e2212837914" width="700"/>
</p>

---

## 🚀 Future Scope

- Integration with **multi-modal sensors** (e.g., Lidar, Radar)
- Deployment on **edge devices** for real-time tunnel inspection
- Extension to **temporal crack detection** in video streams

---

## 🧠 Authors

- [Pediredla Suman](mailto:pediredla22102@iiitnr.edu.in)
- [Bonda Naveen Kumar](mailto:bonda22102@iiitnr.edu.in)
- [Sambangi Chaitanya](mailto:sambangi22100@iiitnr.edu.in)

