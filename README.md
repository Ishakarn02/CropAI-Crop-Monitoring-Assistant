# CropAI-Crop Monitoring Assistant
## Hybrid-CNN-Transformer-Model-for-Optimized-Crop-Management

## Overview
This project presents a hybrid deep learning model combining Convolutional Neural Networks (CNN) and Transformer architectures to optimize crop management. The model assists in the agricultural sector by performing automated crop recognition, evaluating crop health, and predicting specific disease types. The hybrid model utilizes the spatial processing strengths of CNNs and the sequence modeling capabilities of Transformers for precise and efficient crop management.

## Live Demo
You can interact with the model and try out crop recognition, health status evaluation, and disease type prediction in real-time through the following link: https://ishakarn02-cropai-crop-monitoring-assistant-web-cfbgle.streamlit.app/ .

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

## Main Contributions
The key contributions of this project include:
1. *Hybrid CNN-Transformer Model*: A novel approach that combines CNN and Transformer models for agricultural applications, improving crop management processes.
2. *Multi-Stage Crop Management Framework*: The model operates in three distinct stages to identify crops, evaluate health status, and predict diseases.
3. *Optimized Accuracy*: High accuracy in recognizing healthy vs. diseased crops and classifying specific disease types.
4. *Real-World Scalability*: Designed for deployment on farm-level systems, supporting both cloud and edge computing solutions.

## System Overview
The model operates in a multi-stage framework for comprehensive crop management:

### Stage 1: Crop Recognition
In this stage, the model classifies the type of crop from input images. Using CNN layers for spatial feature extraction, the model identifies different crops based on their visual characteristics.

### Stage 2: Health Status Evaluation
Once the crop is recognized, the health status is assessed. The model distinguishes between healthy crops and those showing signs of disease or stress. Transformer layers analyze contextual and sequential data for a more accurate evaluation.

### Stage 3: Disease Type Prediction
If a crop is found to be diseased, the model identifies the specific disease type. This stage combines the spatial feature extraction of CNNs with the contextual analysis of Transformers for precise disease classification.

## Frontend Integration (Streamlit)
The *Streamlit* frontend is integrated directly into the main file of this project. You can run the entire application (both frontend and backend) through the same script.

### Running the Streamlit Frontend
1. *Install the necessary dependencies* for the project:
   ```bash
   pip install -r requirements.txt
Ensure that Streamlit is installed:

bash
Copy code
pip install streamlit
Run the application:
bash
Copy code
streamlit run croptest.py
This will launch the application, and you can access it in your browser at http://localhost:8501.
In the main.py file, you will find both the Streamlit interface and the backend model integration. The frontend allows users to:

Upload images of crops for recognition, health evaluation, and disease prediction.
View the crop’s health status and predicted disease type.
The backend model is used directly within the same file to process the uploaded crop images and return results.

Dataset Format:
plaintext
Copy code


└── CropAI

    ├── maize

    │   ├── healthy
    │   └── unhealthy
    │       ├── blight
    │       ├── common_rust
    │       └── gray_leaf_spot

    ├── sugarcane

    │   ├── healthy
    │   └── unhealthy
    │       ├── mosaic
    │       ├── redrot
    │       ├── rust
    │       └── yellow

    ├── paddy

    │   ├── healthy
    │   └── unhealthy
    │       ├── bacterial_blight
    │       ├── blast
    │       ├── brown_spot
    │       ├── hispa
    │       ├── leaf_blast
    │       └── tungro

    └── wheat
        ├── healthy
        └── unhealthy
            ├── septoria
            └── stripe_rust
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/Ishakarn02/CropAI-Crop-Monitoring-Assistant.git
cd Hybrid-CNN-Transformer-Model-for-Optimized-Crop-Management
Install required dependencies:

bash
Copy code
pip install -r requirements.txt
Download the dataset and organize it within the project directory as required.

Frontend Setup
Install necessary dependencies for Streamlit if not already installed:
bash
Copy code
pip install streamlit
This will run both the frontend and backend from the same file (web.py), providing a seamless user experience.


Demo Features:
Upload Crop Images: Upload crop images and get instant predictions.
Health Status and Disease Prediction: Get results for crop health (healthy/diseased) and disease type.

Results and Performance
The hybrid model demonstrates high accuracy in all three stages—crop recognition, health evaluation, and disease prediction.

Stage 1: Crop Type Classification – The model achieves an impressive validation accuracy of 98.33%, highlighting its high reliability in differentiating between crops (Maize, Paddy, Sugarcane, and Wheat). For most crops, the precision, recall, and F1 scores are close to or at 1.00, indicating exceptional performance. The model shows particular strength in classifying Maize and Sugarcane accurately, with perfect scores across all metrics, underscoring its accuracy in recognizing these crops.

Stage 2: Health Status Detection – Achieving a validation accuracy of 93.30%, the model demonstrates effective performance in distinguishing Healthy from Unhealthy crops. The model performs especially well for the Unhealthy class, with precision and recall around 0.95–0.97, indicating high sensitivity to identifying crop health issues. Healthy crops also show strong results, with an F1 score of 0.83, affirming the model's consistent capability in assessing crop health status accurately.

Stage 3: Disease Detection – With a validation accuracy of 83.80%, the model effectively identifies specific crop diseases, showing consistent scores in precision, recall, and F1 (approximately 0.84–0.85). The weighted average metrics across disease categories also remain high, confirming balanced and stable performance.


Authors
Primary Authors:
[Isha Karn] - Email: [ikarn02@gmail.com]
[Niharika Jain] - Email: [nj180903@gmail.com]
[Kritika Giri] - Email: [kritikagiri03@gmail.com]
