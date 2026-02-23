# 🚆 Railway Track Defect Detection

## 📌 Overview

This project builds a deep learning model to classify railway track images as **Defective** or **Non-Defective** using transfer learning.

The model is implemented using TensorFlow and leverages a pre-trained InceptionResNetV2 backbone with a custom attention-based classification head.

---

## 📂 Dataset

- **Total Images:** 800  
- **Classes:** Defective / Non-Defective  
- **Image Size:** 380 × 380  
- **Split:** Train / Validation / Test  

**Dataset Source:**  
Kaggle – Railway Track Fault Detection Dataset  
https://www.kaggle.com/datasets/ashikadnan/railway-track-fault-detection-dataset1-rail  

---

## 🧠 Model Architecture

### 🔹 Base Model
- Pre-trained InceptionResNetV2 (ImageNet weights)
- Top layers removed
- Feature extraction using transfer learning

### 🔹 Custom Head
- Global Average Pooling
- Custom Multi-Head Attention block
- Skip connection
- Dense layers with L2 regularization
- Gaussian Noise for robustness
- Sigmoid output layer (Binary Classification)

![Model Architecture](https://github.com/user-attachments/assets/68fb3376-a700-44de-b484-23f213bf6e32)

---

## ⚙️ Training Details

- **Optimizer:** Adam (learning rate = 1e-4)  
- **Loss Function:** Binary Crossentropy  
- **Batch Size:** 16  
- **Epochs:** 70  
- **Gradient Clipping:** Enabled  

### 🔹 Callbacks
- ReduceLROnPlateau  
- EarlyStopping  
- ModelCheckpoint  

### 🔹 Evaluation Metrics
- Accuracy  
- AUC  
- Precision  
- Recall  

---

## 📊 Results

> Replace the placeholder values below with your actual performance metrics.

- **Validation Accuracy:** XX%  
- **Validation AUC:** XX  
- **Precision:** XX  
- **Recall:** XX  

(Add confusion matrix / ROC curve image here if available)

---

## 🚀 Future Improvements

- Fine-tuning upper layers of the base model  
- Improved spatial attention mechanism  
- Deployment using Flask or FastAPI  
- Real-time railway inspection integration  

---

## 👨‍💻 Author

Your Name  
M.Tech CSE (AI/ML)





