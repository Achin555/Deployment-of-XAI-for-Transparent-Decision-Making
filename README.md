# 🧠 Deployment of XAI for Transparent Decision Making

## 📌 Overview
This project implements an Explainable AI (XAI) system to classify brain tumors from MRI images, ensuring **transparency and interpretability** of model decisions. Using **LIME** and **Grad-CAM**, we visualize why the model made a certain prediction — critical for trust in medical diagnosis systems.

> ✅ 90%+ Classification Accuracy  
> ✅ Applied LIME for feature-level interpretability  
> ✅ Used Grad-CAM for regional explanations  
> ✅ Built a Streamlit-based interactive web app

---

## 🗂️ Dataset

- **Source**: [Kaggle – Brain Tumor Classification Dataset](https://www.kaggle.com/datasets)
- **Preprocessing**:
  - Images resized to 224×224 or 256×256
  - Normalization and augmentation applied
  - ~3000 total images used (1500 Tumor / 1500 No Tumor)

---

## 🛠️ Technologies Used

| Tool / Library    | Purpose                              |
|------------------|--------------------------------------|
| Python           | Core programming language            |
| TensorFlow/Keras | Deep learning model training         |
| OpenCV           | Image preprocessing                  |
| Matplotlib       | Visualization of results             |
| LIME             | Local explanation technique          |
| Grad-CAM         | CNN-based attention visualization    |
| Streamlit        | Model Deployment UI                  |
| Scikit-learn     | Metrics and preprocessing            |

---

## 🧪 Model Architecture

We trained two models: **VGG16 (pre-trained)** and a **Custom CNN**, optimized for binary classification (tumor/no tumor):

- **Input Size**: 224x224 pixels
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Architecture**: Conv2D → MaxPool → Conv2D → MaxPool → Flatten → Dense → Sigmoid
- **Accuracy Achieved**: **90%+**

---

## 📷 Sample Visual Explanations

### 🧠 MRI Input Images
![MRI Images](images/mri_comparison.png)

### 🔍 LIME Explanation

| VGG16 LIME | Custom Model LIME |
|------------|-------------------|
| ![LIME VGG16](images/lime_vgg16.png) | ![LIME Custom](images/lime_custom.png) |

### 🔥 Grad-CAM Explanation

| VGG16 Grad-CAM | Custom Model Grad-CAM |
|----------------|------------------------|
| ![Grad-CAM VGG16](images/gradcam_vgg16.png) | ![Grad-CAM Custom](images/gradcam_custom.png) |

---

## 🚀 Getting Started

### 🔧 Installation

```bash
git clone https://github.com/Achin555/Deployment-of-XAI-for-Transparent-Decision-Making.git
cd Deployment-of-XAI-for-Transparent-Decision-Making
pip install -r requirements.txt
