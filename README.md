
# 🧠 Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers

This project enhances the YOLOv8n architecture for brain tumor detection using **three advanced attention mechanisms**:  
✔ SimAM (Simple Attention Module)  
✔ Residual Attention  
✔ Tiled Squeeze-and-Excite (TSE)

These mechanisms improve feature extraction, highlight important tumor regions, and boost overall detection accuracy while keeping the model lightweight and fast.

---

## 📌 Overview

Brain tumor detection from MRI scans is a challenging task due to variations in tumor size, shape, and position. To improve detection performance, this project integrates multiple attention layers into the YOLOv8n backbone to make the model more sensitive to tumor-specific features.

Attention helps the model identify *where to focus* and *what features to amplify*, resulting in better localization and classification of Glioma, Meningioma, and Pituitary tumors.

---

## 🎯 Objectives

- **Detect & Classify:** Multi-class detection of Glioma, Meningioma, and Pituitary tumors.  
- **Enhance:** Improve YOLOv8n performance using custom attention modules.  
- **Compare:** Observe performance differences between spatial, residual, and channel-based attention mechanisms.  
- **Deploy:** Build a model suitable for real-time or near real-time clinical assistance.

---

## 🧩 Methodologies Implemented

We enhanced the YOLOv8n (Nano) model by integrating the following attention mechanisms:

### 🔹 1. SimAM (Simple Attention Module)
A parameter-free spatial attention mechanism that identifies important neurons by computing neuron "energy."  
✔ Highlights subtle tumor regions  
✔ No extra parameters added  
✔ Efficient for real-time applications

### 🔹 2. Residual Attention
Uses trunk and mask branches to create multi-scale attention refinement.  
✔ Identifies tumors across multiple resolutions  
✔ Suppresses irrelevant background  
✔ Maintains gradient flow through residual connections

### 🔹 3. Tiled Squeeze-and-Excite (TSE)
A channel attention module that computes channel importance using **local spatial tiles** instead of global pooling.  
✔ Retains local tumor-relevant information  
✔ Improves channel discrimination  
✔ Lightweight and hardware-friendly

---

## 🧬 Dataset

**Source:** Medical Image Brain Tumor Dataset (Figshare / Kaggle)

**Processing Steps:**  
- Resized all images to **640×640**  
- Normalized pixel values  
- Split into **Train / Validation / Test** sets  

### **Classes:**
- **0 – Glioma**  
- **1 – Meningioma**  
- **2 – Pituitary Tumor**

---

## 🚀 Installation
## Prerequisites

Ensure the following are installed:

- Python **3.8+**
- PyTorch  
- Ultralytics (YOLOv8)  
- OpenCV  
- NumPy  
- Matplotlib

## setup
Clone the repository
```bash
git clone https://github.com/jaheer345/Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers.git
cd Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers

