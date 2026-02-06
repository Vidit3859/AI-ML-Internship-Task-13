# Task 13 — PCA Dimensionality Reduction

## Objective
Understand and implement Principal Component Analysis (PCA) for dimensionality reduction and compare model performance before and after feature compression.

---

## Tools Used
- Python
- Scikit-learn
- Matplotlib
- NumPy

---

## Dataset
Sklearn Digits Dataset

- Samples: 1797
- Features: 64
- Classes: 10 digits

---

## Steps Performed

### 1. Load Dataset
Loaded digits dataset from sklearn.

### 2. Feature Scaling
Used StandardScaler to normalize features.

### 3. Apply PCA
Tested PCA with:
- 2 components
- 10 components
- 30 components
- 50 components

### 4. Explained Variance
Measured variance retained for each configuration.

### 5. Cumulative Variance Plot
Plotted cumulative explained variance vs components.

### 6. Dimensionality Reduction
Reduced dataset from 64 features to 30 features.

### 7. Logistic Regression (Original Data)
Trained model on full dataset.

### 8. Logistic Regression (Reduced Data)
Trained model on PCA dataset.

### 9. PCA Visualization
Created 2D PCA scatter plot.

---

## Results

Original features: 64  
Reduced features: 30  

Original Accuracy: ~97%  
Reduced Accuracy: ~96–97%

PCA preserved most useful information while reducing dimensionality.

---

## Key Learning
PCA reduces feature space while retaining maximum variance, improving efficiency with minimal accuracy loss.

---

## Interview Questions (Answers)
- What problem does PCA solve?
PCA reduces dataset dimensionality while preserving maximum variance.
- What is explained variance?
It measures how much information from the original dataset is retained by principal components.
- Why is scaling required for PCA?
Because PCA is variance-based. Features with larger scale would dominate without scaling.

---

## PCA vs Feature Selection
- PCA → creates new features
- Feature selection → selects existing features

---

## PCA limitations
- Reduces interpretability
- Linear method
- Can lose information
- Sensitive to scaling

---
