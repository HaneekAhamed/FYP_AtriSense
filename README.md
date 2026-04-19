# AtriSense
FYP 2026
# AtriSense: A Hybrid Machine Learning–Based Atrial Fibrillation Detection System Using Multi-Lead ECG Data

AtriSense is a machine learning–based web application developed to detect **Atrial Fibrillation (AF)** using structured **12-lead ECG data** together with patient-related information.  
The system was developed as part of an academic research project and compares multiple machine learning models, including **K-Nearest Neighbors (KNN)**, **Random Forest (RF)**, **Weighted Soft Voting**, and **Stacking Ensemble Learning**.

The best-performing model was the **Stacking Ensemble**, which achieved the highest overall classification performance.

---

## Project Overview

Atrial Fibrillation (AF) is one of the most common cardiac arrhythmias and is associated with serious complications such as stroke, heart failure, and increased mortality. Early detection is important because AF may occur intermittently and may remain asymptomatic for long periods.

This project aims to support AF detection using a structured machine learning workflow with:

- ECG lead values
- Patient demographic and physical features
- Model comparison and evaluation
- Web-based prototype deployment

---

## Features

- Uses **16 structured input features**
  - **12 ECG leads**: I, II, III, aVR, aVL, aVF, V1, V2, V3, V4, V5, V6
  - **4 additional features**: Age, Gender, Height, Weight
- Data preprocessing and feature engineering pipeline
- Multiple machine learning models tested
- Ensemble learning for better performance
- Flask-based web application for prediction
- Prototype system for AF detection

---

## Models Used

The following models were implemented and evaluated:

1. **K-Nearest Neighbors (KNN)**
2. **Random Forest (RF)**
3. **Weighted Soft Voting Ensemble**
4. **Stacking Ensemble**

### Best Model
The **Stacking Ensemble** achieved the best performance in this project.

---

## Model Performance

| Model | Accuracy | Precision | Recall | F1-score |
|------|----------|-----------|--------|----------|
| KNN | 0.8205 | 0.8153 | 0.8175 | 0.8162 |
| Random Forest | 0.8864 | 0.8883 | 0.8799 | 0.8834 |
| Weighted Soft Voting | 0.8847 | 0.8866 | 0.8783 | 0.8819 |
| Stacking Ensemble | 0.8887 | 0.8879 | 0.8843 | 0.8860 |

---

## Project Structure

```bash
AtriSense/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── feature_engineering.ipynb
│   ├── RF_KNN_Model_and_Ensemble_Model.ipynb
│
├── model/
│   ├── model_pickel.pkl
│
├── app/
│   ├── app.py
│   ├── templates/
│   ├── static/
│
├── requirements.txt
├── README.md
└── LICENSE
