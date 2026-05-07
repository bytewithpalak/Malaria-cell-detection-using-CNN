# 🦠 Malaria Cell Detection using Deep Learning (EfficientNetB0)

A deep learning-based medical image classification project that detects whether a blood cell image is **Parasitized** or **Uninfected** using **EfficientNetB0** and TensorFlow.

---

## 📌 Project Overview

Malaria is a life-threatening disease caused by parasites transmitted through infected mosquitoes. Early and accurate diagnosis is critical.

This project uses a **Convolutional Neural Network (CNN)** with **Transfer Learning (EfficientNetB0)** to automatically classify microscopic blood smear images into:

- ✅ Uninfected
- 🦠 Parasitized

The model was trained and tested using TensorFlow/Keras in Google Colab. :contentReference[oaicite:0]{index=0}

---

# 🖼️ Sample Dataset Images

<img width="862" height="617" alt="image" src="https://github.com/user-attachments/assets/250f4295-d060-440f-b36c-5c17289b7e24" />


---

# 📂 Dataset

Dataset Used: **Cell Images for Detecting Malaria**

🔗 Dataset Link:  
https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria

- Total Images: 27,000+
- Classes:
  - Parasitized
  - Uninfected

The dataset was downloaded using KaggleHub in Google Colab. :contentReference[oaicite:1]{index=1}

---

# 🚀 Technologies Used

- Python
- TensorFlow / Keras
- EfficientNetB0
- OpenCV
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

# 🧠 Model Architecture

The project uses **Transfer Learning** with EfficientNetB0.

### Architecture:
- EfficientNetB0 (pretrained on ImageNet)
- Global Average Pooling
- Dense Layer (ReLU)
- Dropout Regularization
- Output Layer (Sigmoid)

Training was performed in 2 phases:
1. Training only the classifier head
2. Fine-tuning last layers of EfficientNetB0 :contentReference[oaicite:2]{index=2}

---

# ⚙️ Data Augmentation

To improve generalization, the following augmentations were used:

- Rotation
- Zoom
- Width/Height Shift
- Horizontal Flip
- Vertical Flip

:contentReference[oaicite:3]{index=3}

---

# 📊 Results

## ✅ Final Performance

| Metric | Score |
|--------|--------|
| Accuracy | 92% |
| AUC Score | 0.97 |
| Precision | 0.92 |
| Recall | 0.92 |

Classification report generated after evaluation showed strong performance on both classes. :contentReference[oaicite:4]{index=4}

---


---

# 🔥 Grad-CAM Visualization

Grad-CAM was used to visualize which regions of the blood cell image influenced predictions.

This improves model interpretability and helps understand CNN decision-making. :contentReference[oaicite:6]{index=6}

---

# 📊 Confusion Matrix

The confusion matrix showed strong classification capability for both infected and uninfected cells. :contentReference[oaicite:7]{index=7}
<img width="576" height="413" alt="image" src="https://github.com/user-attachments/assets/d4db87ae-d0f9-468c-bc9a-b96b28fa5f24" />

---


