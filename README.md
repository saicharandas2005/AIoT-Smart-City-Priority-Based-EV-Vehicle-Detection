# 🚑 Priority Vehicle Classification for Smart EV Charging & AIoT

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch)
![YOLO](https://img.shields.io/badge/YOLO-Ultralytics-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

> **Research Codebase for:**
> 1. *Deep Learning Enabled Vehicle Classification System for EV Charging Station Management* (ICONAT 2025)
> 2. *AIoT Enabled Vehicle Classification Using Ensemble, Deep Learning, and Transformer Models* (ACOIT 2025)

## 📖 Overview
The rapid adoption of Electric Vehicles (EVs) has introduced operational challenges, specifically regarding queue management and prioritization at charging stations. This repository contains the source code, experiments, and model comparisons for an **Intelligent Vehicle Classification System**.

The system is designed to automatically detect and classify vehicles into priority groups (Emergency, Government/VIP, Civilian) to facilitate dynamic resource allocation in Smart Cities and EV Charging Stations.

---

## 🔬 Research & Methodologies

This repository covers two distinct approaches to solving the vehicle prioritization problem:

### Study 1: Object Detection Approaches (ICONAT 2025)
Focuses on real-time detection and localization of priority vehicles.
* **Models Evaluated:**
    * **YOLOv8m:** Anchor-free, single-stage detector.
    * **SSD300-VGG16:** Single Shot MultiBox Detector with VGG backbone.
    * **RF-DETR (Base):** Transformer-based detector using DINOv2 backbone.
* **Key Result:** **RF-DETR** achieved the highest performance with an **mAP@0.5 of 0.986**.

### Study 2: AIoT Classification & Ensembles (ACOIT 2025)
Focuses on lightweight classification for edge devices and robust ensemble learning.
* **Feature Extraction:** EfficientNetB0 + PCA (for ML models).
* **Ensemble Models:**
    * *HCE (Hybrid Classical Ensemble):* KNN + Decision Tree + Gradient Boosting.
    * *BEF (Boosting Ensemble Framework):* XGBoost + LightGBM + CatBoost.
* **Deep Learning & Transformers:**
    * **YOLOv11m:** Optimized for real-time edge detection.
    * **RetinaNet:** Restructured for classification.
    * **Vision Transformer (ViT-B/16):** Attention-based global context processing.
* **Key Result:** **ViT-B/16** provided the best reliability (90.55% Accuracy) with superior class separation.

---

├── datasets/                        # Scripts for Roboflow data download/prep
└── assets/                          # Confusion matrices and results graphs

