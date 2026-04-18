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
3)CNN For CIFAR DATASET

Implemented a Convolutional Neural Network (CNN) using PyTorch to classify images from the CIFAR-10 dataset.

Model-:
3 Convolutional layers: 3→32 → 32→64 → 64→128
Spatial size reduces: 32→16→8→4
Final feature size: 2048
Fully connected layers for classification (10 classes)

Training-:
Loss Function: CrossEntropyLoss
Optimizer: Adam
Epochs: 10

Evaluation-:
Predictions obtained by selecting the class with highest score
Accuracy calculated by comparing predicted and actual labels

Result-:
Achieved ~75% accuracy on CIFAR-10


4)DOg vs Cat Classification Using CNN
This project implements a Convolutional Neural Network (CNN) from scratch using PyTorch to classify images of cats and dogs.

Images were preprocessed by resizing to 32×32 and normalizing pixel values. The model consists of three convolutional layers where feature depth increases (3 → 32 → 64 → 128) while spatial dimensions decrease through max pooling (32 → 16 → 8 → 4). This allows the network to learn hierarchical features from basic edges to complex object patterns.

The final feature map (4×4×128) is flattened and passed through fully connected layers for binary classification.

The model was trained using CrossEntropyLoss and the Adam optimizer over 8 epochs, achieving an accuracy of 82.13% on the dataset.

Key Highlights
Learned hierarchical feature extraction using CNN
Demonstrated spatial reduction with increasing feature depth
Applied effective preprocessing and training strategies

5)RNN For Sentinal Analysis


This project performs sentiment analysis on the IMDB movie review dataset using a Recurrent Neural Network (RNN).

🔹 Workflow
Text preprocessing (remove URLs, HTML tags, punctuation, stopwords, stemming)
Feature extraction using TF-IDF
Data conversion using TensorDataset and DataLoader
Model building using RNN + Fully Connected layer
Training using BCELoss and Adam optimizer (10 epochs)
Evaluation using accuracy metric
🔹 Model Details
RNN with hidden size = 128
Final layer: Linear (hidden → 1)
Activation: Sigmoid for binary classification
🔹 Result
Achieved 85.78% accuracy on test data
🔹 Tech Stack
Python
PyTorch
NLP (TF-IDF, preprocessing)

