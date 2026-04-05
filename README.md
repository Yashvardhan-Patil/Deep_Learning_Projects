#  Deep Learning Projects - ANN (PyTorch)

This repository contains my Deep Learning projects where I implemented Artificial Neural Networks (ANN) using PyTorch for both regression and classification tasks.

---

##  Projects Included

### 1️⃣ ANN for Regression (Power Plant Dataset)

 **Objective:**
Predict electrical energy output (PE) based on environmental conditions.

**Input Features:**
- Ambient Temperature (AT)
- Exhaust Vacuum (V)
- Ambient Pressure (AP)
- Relative Humidity (RH)

**Target:**
- Electrical Energy Output (PE)

 **Implementation Steps:**
- Data loading and preprocessing  
- Feature-target split  
- Train-test split  
- Applied StandardScaler  
- Converted data into PyTorch tensors  
- Used TensorDataset and DataLoader (batch size = 32)  

 **Model:**
- 2 Hidden Layers with ReLU activation  
- Optimizer: Adam  
- Loss Function: MSE Loss  

 **Results:**
- MSE: 17.74  
- R² Score: 0.93  

---

### 2️⃣ ANN for Classification (Date Fruit Dataset)

 **Objective:**
Classify different types of date fruits into 7 categories.

Input Features:**
- Area, Perimeter, Major Axis, Minor Axis  
- Eccentricity, Equidiameter, Solidity  
- Convex Area, Extent, Aspect Ratio  
- Color Features (RG, RB, RR)  
- Entropy Features (RG, RB, RR)  
- Texture Features (Daubechies)

 **Implementation Steps:**
- Data preprocessing  
- Label Encoding of fruit types (e.g., Berhi)  
- Train-test split  
- Applied StandardScaler  
- Converted data into tensors  
- Used TensorDataset and DataLoader (batch size = 32)  

**Model:**
- 2 Hidden Layers with ReLU activation  
- Loss Function: CrossEntropyLoss  
- Optimizer: Adam  

 **Results:**
- Accuracy: 94%  

---
## Saved Models
This Repository includes trained model files
-best_model_of_regression.pt=Trained ANN model for regression
Note-
These are pytorch binary files and cannot be previewde directly on github.
##  Tech Stack
- Python  
- PyTorch  
- NumPy  
- Pandas  
- Scikit-learn  

---

##  Key Learnings
- End-to-end ANN implementation  
- Data preprocessing and feature scaling  
- Batch training using DataLoader  
- Forward and backward propagation  
- Model evaluation using regression and classification metrics  

---

## 📎 Future Improvements
- Hyperparameter tuning  
- Dropout for regularization  
- Model optimization  

---

