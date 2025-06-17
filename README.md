# 🧠 Brain Tumor MRI Classification Using Xception

This project focuses on the classification of brain MRI scans into four categories: **Glioma**, **Meningioma**, **Pituitary Tumor**, and **No Tumor**. A deep learning model based on the **Xception architecture** is used to achieve high diagnostic accuracy in medical imaging.

---

## 🎯 Project Goal

To develop a deep learning-based medical image classifier capable of accurately detecting and classifying brain tumors using MRI scans. The aim is to assist in fast and reliable diagnosis.

---

## 🧠 Model and Performance

- Built upon the **Xception model** with additional custom dense layers and dropout for regularization.
- Achieved **over 99% accuracy** on both validation and test datasets.
- Outperforms traditional CNNs in both precision and generalization.

---

## ⚙️ Training Configuration

- **Optimizer**: Adamax  
- **Loss Function**: Categorical Cross-Entropy  
- **Regularization**: Dropout and EarlyStopping  
- **Data Preparation**: Data augmentation using ImageDataGenerator  
- **Epochs**: 10  
- **Image Size**: 299x299x3

---

## 📊 Results

- Achieved high classification metrics across all tumor types.
- Evaluated using:
  - Accuracy
  - Classification Report
  - Confusion Matrix

---

## 🧰 Technologies Used

- Python  
- TensorFlow  
- Keras  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  

---

## 📁 Dataset
- https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data
- The dataset consists of labeled MRI images categorized into four classes.
- It is preprocessed and split into training, validation, and test sets using stratified sampling.

---
