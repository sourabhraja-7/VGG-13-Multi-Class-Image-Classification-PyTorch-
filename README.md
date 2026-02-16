

# VGG-13 Multi-Class Image Classification (PyTorch)

> A from-scratch VGG-13 implementation adapted for 28×28 images, classifying across 36 categories with >85% accuracy.

---

## 📋 Overview

This project implements the **VGG-13 Convolutional Neural Network** architecture from scratch using PyTorch and applies it to classify images into **36 categories**.

The original VGG-13 architecture was modified to accommodate smaller input dimensions and the target number of classes.

| Property       | Details   |
|----------------|-----------|
| Classes        | 36        |
| Total images   | 100,800   |
| Image size     | 28×28     |

---

## ✨ Features

- 🏗️ Full VGG-13 implementation from scratch
- 🔄 Architecture adapted for 28×28 images
- 🏷️ Multi-class image classification (36 categories)
- 📉 Model training and evaluation pipeline
- 📊 Accuracy and loss visualization

---

## 📁 Project Structure

```
VGG13-Image-Classification/
│
├── VGG-Implementation.ipynb   # Main training notebook
├── README.md                  # Project documentation
└── requirements.txt           # Dependencies
```

---

## 🏗️ VGG-13 Architecture

```
Input Image (28×28)
     │
     ▼
Conv → ReLU
Conv → ReLU
     │
   MaxPool
     │
     ▼
Conv → ReLU
Conv → ReLU
     │
   MaxPool
     │
     ▼
Conv → ReLU
Conv → ReLU
     │
   MaxPool
     │
     ▼
Fully Connected Layers
     │
     ▼
Output Layer (36 classes)
```

| Component     | Value              |
|---------------|--------------------|
| Loss Function | `CrossEntropyLoss` |
| Optimizer     | `Adam`             |

---

## 🔧 Modifications from Original VGG-13

| Component             | Original VGG-13  | This Implementation |
|-----------------------|------------------|----------------------|
| Input size            | 224×224          | 28×28               |
| Pooling layers        | Standard         | Adjusted             |
| Fully connected layers| Standard         | Adjusted             |
| Output classes        | 1,000            | 36                   |

---

## 📊 Results

| Metric        | Value    |
|---------------|----------|
| Test Accuracy | **>85%** |
| Convergence   | Stable   |

### Visualizations Included:
- 📈 Accuracy curves
- 📉 Loss curves
- 🟦 Confusion matrix

---

## 🚀 How to Run

**1. Install dependencies:**
```bash
pip install -r requirements.txt
```

**2. Launch the training notebook:**
```bash
jupyter notebook VGG-Implementation.ipynb
```

---

## 🛠️ Technologies Used

| Tool          | Purpose                    |
|---------------|----------------------------|
| Python        | Core language              |
| PyTorch       | Model building & training  |
| Torchvision   | Dataset utilities          |
| NumPy         | Numerical operations       |
| Matplotlib    | Plotting & visualization   |
| Scikit-learn  | Evaluation metrics         |

---
