# Lung Cancer Detection using Feature Engineering & Ensemble Learning

---

## Project Overview

This project focuses on detecting lung cancer from CT scan images using classical computer vision + machine learning ensemble methods.

Instead of deep learning, the system uses feature engineering techniques to convert images into numerical data, followed by ensemble ML models for classification.

The final system can classify lung CT images into:

- Normal  
- Benign  
- Malignant  

---

## Objective

The main goal of this project is:

- To build a non-deep learning approach for medical image classification  
- To extract meaningful features from CT scan images  
- To apply and compare multiple ensemble learning models  
- To build a complete end-to-end ML pipeline  

---

## Methodology

The project follows this pipeline:
- Image Input
- Preprocessing (Resize + Grayscale + Noise Removal)
- Feature Extraction
- Feature Vector Dataset
- ML Model Training
- Ensemble Learning (Bagging, Boosting, Stacking)
- Final Prediction


---

## Feature Engineering Techniques Used

Each image is converted into a feature vector using:

### 1. HOG (Histogram of Oriented Gradients)
- Captures shape and structure information  

### 2. GLCM (Texture Features)
- Contrast  
- Homogeneity  
- Energy  
- Correlation  

### 3. Edge Detection (Canny)
- Extracts boundary and structural information  

### 4. Statistical Features
- Mean  
- Standard Deviation  
- Variance  

---

## Machine Learning Models

### Bagging Models
- Random Forest  
- Extra Trees Classifier  

### Boosting Models
- XGBoost  
- AdaBoost  

### Stacking Model (Best Model)
- **Base Models:** Random Forest + XGBoost  
- **Meta Model:** Logistic Regression  

---

## Best Model

After evaluation, **Stacking Classifier** performed best and was selected as the final model.

---

## Evaluation Metrics

All models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-Score  

Since this is a medical dataset, **Recall was given high importance** to reduce false negatives.


---

## Final Output

The model generates a visual prediction report:

- 10 sample CT images  
- Predicted labels:  
  - Normal  
  - Benign  
  - Malignant  
