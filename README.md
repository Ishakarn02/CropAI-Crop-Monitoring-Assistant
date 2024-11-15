# CropAI: Crop Monitoring Assistant
## Hybrid-CNN-Transformer-Model-for-Optimized-Crop-Management

---

## Overview
This project presents a hybrid deep learning model combining **Convolutional Neural Networks (CNN)** and **Transformer** architectures to optimize crop management. The model assists the agricultural sector by automating crop recognition, evaluating crop health, and predicting specific disease types. By leveraging the spatial processing strengths of CNNs and the sequence modeling capabilities of Transformers, the model achieves precise and efficient crop management.

---

## Live Demo
Try the application in real-time: [CropAI Live Demo](https://ishakarn02-cropai-crop-monitoring-assistant-web-cfbgle.streamlit.app/)

---

## Table of Contents
- [Main Contributions](#main-contributions)
- [System Overview](#system-overview)
  - [Stage 1: Crop Recognition](#stage-1-crop-recognition)
  - [Stage 2: Health Status Evaluation](#stage-2-health-status-evaluation)
  - [Stage 3: Disease Type Prediction](#stage-3-disease-type-prediction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results and Performance](#results-and-performance)
- [Authors](#authors)

---

## Main Contributions
1. **Hybrid CNN-Transformer Model**: A novel approach combining CNN and Transformer models for agricultural applications.
2. **Multi-Stage Framework**: Identifies crops, evaluates health status, and predicts diseases in three stages.
3. **High Accuracy**: Robust performance in crop recognition, health assessment, and disease prediction.
4. **Real-World Scalability**: Compatible with cloud and edge computing systems for farm-level deployment.

---

## System Overview
The model operates in a multi-stage framework for comprehensive crop management:

### Stage 1: Crop Recognition
- **Goal**: Classify crop type from input images.
- **Approach**: Uses CNN layers for spatial feature extraction to identify crops based on visual characteristics.

### Stage 2: Health Status Evaluation
- **Goal**: Assess the health status of the identified crop.
- **Approach**: Transformer layers analyze contextual and sequential data for accurate evaluation.

### Stage 3: Disease Type Prediction
- **Goal**: Identify specific diseases affecting the crop.
- **Approach**: Combines CNN's spatial feature extraction with Transformer's contextual analysis for precise disease classification.

---

## Installation
### Step 1: Clone this repository
```bash
git clone https://github.com/Ishakarn02/CropAI-Crop-Monitoring-Assistant.git

### Step 2: Install dependencies
```bash
pip install -r requirements.txt
