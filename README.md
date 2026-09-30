# 🌾 Rice Image Classification using Convolutional Neural Network (CNN)

![Python](https://img.shields.io/badge/Python-3873A9?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)

**Author:** Ahmad Izzuddin Ulinnuha[cite: 2]  
**Project:** Machine Learning Development Submission (Image Classification)[cite: 2]  

---

## 📌 Project Overview
This project implements a **Convolutional Neural Network (CNN)** architecture built with **TensorFlow/Keras** to classify 5 varieties of rice images[cite: 2]. The model is trained and optimized to achieve an accuracy target **above 95%** on both training and test datasets[cite: 2].

---

## 📊 Dataset Overview

- **Dataset Source:** [Rice Image Dataset (Kaggle)](https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset)[cite: 2]
- **Total Images:** 75,000 images[cite: 2]
- **Classes (5 Varieties):** `Arborio`, `Basmati`, `Ipsala`, `Jasmine`, `Karacadag`[cite: 2]

### Dataset Split
| Subset | Percentage |
| :--- | :--- |
| **Train Set** | 80% |[cite: 2]
| **Validation Set** | 10% |[cite: 2]
| **Test Set** | 10% |[cite: 2]

---

## 🏗️ Model Architecture

The model is built using the **Keras Sequential API** with the following layer structure[cite: 2]:

- **Feature Extraction:** 3× `Conv2D` layers for visual feature extraction[cite: 2].
- **Dimensionality Reduction:** `MaxPooling2D` layers following convolution blocks[cite: 2].
- **Regularization:** `Dropout(0.5)` layer to prevent overfitting[cite: 2].
- **Classification Head:** `Dense` layer with `Softmax` activation for multi-class classification[cite: 2].

---

## ⚙️ Training & Performance

- **Optimizer:** Adam Optimizer[cite: 2]
- **Loss Function:** `categorical_crossentropy`[cite: 2]
- **Custom Callbacks:** Automatically halts training when training and validation accuracy exceed **96%**[cite: 2].
- **Final Performance:**
  - **Training Accuracy:** > 95%[cite: 2]
  - **Testing Accuracy:** > 95%[cite: 2]

---

## 📁 Directory Structure

```text
submission/
├── tfjs_model/           # Model exported in TensorFlow.js format
├── tflite/               # Model exported in TF-Lite format (.tflite & label.txt)
├── saved_model/          # Model exported in SavedModel format (.pb)
├── notebook.ipynb        # Jupyter Notebook for experimentation & training
├── README.md             # Project documentation
└── requirements.txt      # Python dependencies
```[cite: 2]

---

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/username/rice-image-classification.git](https://github.com/username/rice-image-classification.git)
   cd rice-image-classification
