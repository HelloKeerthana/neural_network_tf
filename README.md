# Neural Network Model for Wine Data Classification

## Overview
this project uses a neural network to classify wine types based on chemical properties. <br>
the model is built with a dense neural network architecture and incorporates dropout to prevent overfitting.

---

## Model Architecture
- **Standard Scaling:** Applied to training and testing feature data using `StandardScaler` from `sklearn.preprocessing`.  
- **Neural Network Layers:**
  - Dense Layer 1: `ReLU` activation  
  - Dense Layer 2: `ReLU` activation  
  - Dense Output Layer: `Softmax` activation (for multi-class classification)  
- **Dropout:** Regularization to mitigate overfitting.

---

## Dataset
- **Source:** `sklearn.datasets.load_wine()`  
- **Data Features:** Includes chemical properties of different wine types  
- **Target:** Multi-class classification of wine types (0, 1, 2)

---

## Training and Testing
- **Data Splitting:** Training, testing using `train_test_split()` from `sklearn.model_selection`.  
- **Model Training:** Optimizer: Adam for efficient gradient-based optimization, validation set of 0.1
- **Prediction:** Model predicts the wine type based on input features.
- **loss:** sparse categorical entropy function
---

## Visualization
- Graphs for model evaluation:
  - Loss and accuracy curves during training and validation  
  - Confusion matrix for prediction analysis  

---
