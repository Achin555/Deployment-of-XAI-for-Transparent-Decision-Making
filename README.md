# 🧠 Deployment of XAI for Transparent Decision Making

## 📌 Overview
This project implements an Explainable AI (XAI) system to classify brain tumors from MRI images, ensuring **transparency and interpretability** of model decisions, using **LIME** and **Grad-CAM**.

> ✅ 90%+ Classification Accuracy  
> ✅ LIME for pixel‑level explanations  
> ✅ Grad‑CAM for regional attention  
> ✅ Streamlit interface for deployment

---

## 🗂️ Dataset

- **Source**: [Kaggle – Brain Tumor Classification Dataset](https://www.kaggle.com/datasets)
- **Preprocessing**:
  - Resized to 224×224 or 256×256
  - Normalization and augmentation applied
  - ~3000 images total (1500 Tumor / 1500 No Tumor)

---

## 🛠️ Technologies Used

| Tool / Library    | Purpose                              |
|------------------|--------------------------------------|
| Python           | Core programming language            |
| TensorFlow/Keras | Deep learning                        |
| OpenCV           | Image processing                     |
| Matplotlib       | Visualizations                       |
| LIME             | Feature-level interpretability       |
| Grad-CAM         | Region-level visual explanations     |
| Streamlit        | Deployment UI                        |
| Scikit-learn     | Metrics & preprocessing              |

---

## 🧪 Model Architecture

Two models were trained:

- **VGG16** (pre-trained)
- **Custom CNN**

Both use 224×224 input and achieve > 90% accuracy with Adam optimizer and Categorical Crossentropy loss.

---

## 📷 Sample Visual Explanations

### 🧠 MRI Input Images
![MRI Examples](Screenshot%202025-07-11%20002049.png)

### 🔍 LIME Explanation (VGG16)
![LIME Custom CNN Model](Screenshot%202025-07-11%20002116.png)

### 🔍 LIME Explanation (CUSTOM CNN Model)
![LIME VGG16](Screenshot%202025-07-11%20002204.png)

### 🔥 Grad-CAM Explanation (Custom CNN Model)
![Grad-CAM Custom CNN Model](Screenshot%202025-07-11%20002132.png)

### 🔥 Grad-CAM Explanation (VGG16)
![Grad-CAM VGG16](Screenshot%202025-07-11%20002149.png)


---

## 🚀 Getting Started

### 🔧 Installation

```bash
git clone https://github.com/Achin555/Deployment-of-XAI-for-Transparent-Decision-Making.git
cd Deployment-of-XAI-for-Transparent-Decision-Making
pip install -r requirements.txt
