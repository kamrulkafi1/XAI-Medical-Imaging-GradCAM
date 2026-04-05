# Explainable AI (XAI) for Medical Diagnostics

## 📌 Project Overview
This project focuses on the interpretability of Deep Learning models in healthcare. Using **Grad-CAM (Gradient-weighted Class Activation Mapping)**, I visualized the decision-making process of a **ResNet50** model trained on the **HAM10000** (Skin Cancer) dataset. 

The goal is to bridge the gap between AI performance and clinical trust by providing visual evidence of why a model classifies a lesion as malignant or benign.

## 🛠️ Technical Stack
- **Framework:** PyTorch
- **Library:** Captum (Model Interpretability)
- **Dataset:** HAM10000 (Skin Cancer MNIST)
- **Architecture:** ResNet50 (Transfer Learning)

## 📊 Key Results
The following heatmap demonstrates how the model identifies the central features of a skin lesion:

![Grad-CAM Heatmap](results/gradcam_result.png)

## 📖 Methodology
1. **Preprocessing:** Standardizing medical images to 224x224 and normalizing per ImageNet standards.
2. **Backbone:** Utilizing ResNet50's final convolutional layer (`layer4`) to capture high-level semantic information.
3. **Attribution:** Computing gradients of the target class to generate a localization map highlighting important regions.

## 🎓 Academic Application
This project is part of my preparation for **MSc in Data Science/AI** in Germany, focusing on **Reliable and Interpretable Machine Learning.**

[![Kaggle](https://www.kaggle.com/code/kamrulislamkafi/explainable-ai-xai-for-medical-diagnostics)
