📌 Overview

This project builds a deep learning model to classify railway track images as Defective or Non-Defective using transfer learning.
The model uses TensorFlow with a pre-trained InceptionResNetV2 backbone and a custom attention-based classification head.

📂 Dataset

Total Images: 800
Classes: Defective / Non-Defective
Image Size: 380 × 380
Split: Train / Validation / Test
Dataset link:https://www.kaggle.com/datasets/ashikadnan/railway-track-fault-detection-dataset1-rail

🧠 Model Architecture

Pre-trained InceptionResNetV2 (ImageNet weights)
Global Average Pooling
Custom Multi-Head Attention block
Skip connection
Dense layers with L2 regularization
Gaussian Noise
Sigmoid output layer (Binary classification)

<img width="1250" height="786" alt="Screenshot 2025-03-24 at 11 34 06 AM" src="https://github.com/user-attachments/assets/68fb3376-a700-44de-b484-23f213bf6e32" />


⚙️ Training Details

Optimizer: Adam (lr = 1e-4)
Loss: Binary Crossentropy
Batch Size: 16
Epochs: 70
Callbacks:
  ReduceLROnPlateau
  EarlyStopping
  ModelCheckpoint
Metrics:
  Accuracy
  AUC
  Precision
  Recall

📊 Results

(Add your actual numbers here — this is IMPORTANT)

Example:

Validation Accuracy: XX%
Validation AUC: XX
Precision: XX
Recall: XX

(Add confusion matrix / ROC curve image here if available)






