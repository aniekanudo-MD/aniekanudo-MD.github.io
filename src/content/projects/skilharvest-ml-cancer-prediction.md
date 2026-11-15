---
title: "Skilharvest Ml Cancer Prediction"
repo: "aniekanudo-MD/skilharvest_ml_cancer_prediction"
category: "Data Science"
description: "A machine learning application that predicts breast cancer diagnosis using Support Vector Machine (SVM) classification. The model analyzes 23 histology parameters (radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, fractal dimension) to classify tumors as **Benign** or..."
excerpt: "A machine learning application that predicts breast cancer diagnosis using Support Vector Machine (SVM) classification. The model analyzes 23 histology parameters (radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, fractal dimension) to classify tumors as **Benign** or..."
thumbnail: "/default-thumbnail.svg"
githubUrl: "https://github.com/aniekanudo-MD/skilharvest_ml_cancer_prediction"
stars: 0
language: ""
featured: false
priority: 10
tags: []
techStack:
  - "Python"
  - "Scikit-learn"
  - "SVM"
  - "Streamlit"
  - "Pandas"
  - "NumPy"
  - "PIL"
status: "Complete"
liveDemo: ""
features:
  - "**SVM Classification**: Pre-trained Support Vector Machine model for breast cancer diagnosis"
  - "**23 Histology Parameters**: Input cellular measurements including radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension"
  - "**Real-Time Prediction**: Instant classification result (Benign or Malignant) upon form submission"
  - "**Interactive Form**: Streamlit-based input form with expandable parameter section"
  - "**Data Preview**: Displays input data as a dataframe before prediction"
---

# Skilharvest Ml Cancer Prediction

# Cancer Prediction with SVM
**Category:** Data Science  
**Tech Stack:** Python, Scikit-learn, SVM, Streamlit, Pandas, NumPy, PIL  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
A machine learning application that predicts breast cancer diagnosis using Support Vector Machine (SVM) classification. The model analyzes 23 histology parameters (radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, fractal dimension) to classify tumors as **Benign** or **Malignant**. Built with scikit-learn and served through an interactive Streamlit web interface.
## Features
- **SVM Classification**: Pre-trained Support Vector Machine model for breast cancer diagnosis
- **23 Histology Parameters**: Input cellular measurements including radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension
- **Real-Time Prediction**: Instant classification result (Benign or Malignant) upon form submission
- **Interactive Form**: Streamlit-based input form with expandable parameter section
- **Data Preview**: Displays input data as a dataframe before prediction
## Getting Started
### Prerequisites
- Python 3.8+
- uv (recommended) or pip
### Installation
```bash
# Clone the repository
git clone https://github.com/aniekanudo-MD/skilharvest_ml_cancer_prediction.git
cd skilharvest_ml_cancer_prediction
# Install dependencies with uv
uv sync
# or with pip
pip install streamlit pandas numpy scikit-learn pillow
Run the App
streamlit run cancer.py
The app will open in your browser at http://localhost:8501
Project Structure
skilharvest_ml_cancer_prediction/
├── cancer.py              # Streamlit application with input form
├── machine.py             # SVM model logic and prediction pipeline
├── cancer_svm.pkl         # Pre-trained SVM model (pickled)
└── README.md
Model Details
- 
Algorithm: Support Vector Machine (SVM)
- 
Features: 23 histology parameters (radius_mean, texture_mean, perimeter_mean, area_mean, smoothness_mean, compactness_mean, concavity_mean, concave points_mean, symmetry_mean, radius_se, perimeter_se, area_se, concave points_se, radius_worst, texture_worst, perimeter_worst, area_worst, smoothness_worst, compactness_worst, concavity_worst, concave points_worst, symmetry_worst, fractal_dimension_worst)
- 
Output: Benign (non-cancerous) or Malignant (cancerous)
- 
Preprocessing: StandardScaler normalization
How It Works
1. 
Input: User enters 23 cellular measurement values through the Streamlit form
2. 
Preprocessing: Data is standardized using StandardScaler
3. 
Prediction: SVM model classifies the tumor
4. 
Result: Displays "Benign" or "Malignant" diagnosis
License
MIT
