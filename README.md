# 🧠 Deployment of XAI for Transparent Decision Making

## 📌 Overview

This project implements an Explainable AI (XAI) system to classify **brain tumors** from MRI images while ensuring transparency and trust in the model's predictions. Using state-of-the-art techniques like **LIME** and **Grad-CAM**, the model not only performs accurate predictions but also **visualizes the reasoning behind its decisions** — a critical requirement in healthcare applications.

- ✅ Achieved **90%+ classification accuracy**
- ✅ Applied **LIME** for local feature importance visualization
- ✅ Used **Grad-CAM** to highlight key regions in MRI images
- ✅ Built a deployment-ready application using **Streamlit**

---

## 🗂️ Dataset

- **Source**: Kaggle  
- **Link**: [Brain Tumor Classification Dataset](https://www.kaggle.com/datasets)
- The dataset contains MRI images categorized into three tumor types:
  - **Glioma Tumor**
  - **Meningioma Tumor**
  - **Pituitary Tumor**

Each class has hundreds of labeled images, enabling robust supervised training.

---

## 🛠️ Technologies Used

| Tool / Library      | Purpose                             |
|---------------------|-------------------------------------|
| Python              | Core programming language           |
| TensorFlow / Keras  | Deep learning framework             |
| OpenCV              | Image processing                    |
| Matplotlib / Seaborn| Visualization                       |
| LIME                | Model interpretability              |
| Grad-CAM            | Visual explanations of CNNs         |
| Streamlit           | UI for deployment                   |
| Scikit-learn        | Metrics, preprocessing              |

---

## 🧪 Model Architecture

A Convolutional Neural Network (CNN) was trained from scratch using MRI images as input. The model was evaluated on accuracy and interpretability, and it demonstrated high performance with the following characteristics:

- **Input Size**: 224x224 MRI images
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Accuracy**: **90%+** on test set
- **Explainability**: LIME + Grad-CAM overlays

---

## 📷 Sample Visual Explanations

| MRI Image | Grad-CAM Output | LIME Output |
|-----------|------------------|--------------|
| ![MRI](assets/sample_mri.png) | ![GradCAM](assets/sample_gradcam.png) | ![LIME](assets/sample_lime.png) |

These outputs help clinicians verify **why** a prediction was made by focusing on image regions or pixel importance.

---

## 🚀 Getting Started

### 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Achin555/Deployment-of-XAI-for-Transparent-Decision-Making.git
   cd Deployment-of-XAI-for-Transparent-Decision-Making
****
