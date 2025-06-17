# Brain Tumor MRI Classification (Custom CNN, ResNet50, VGG16)

This project aims to classify brain MRI images into four categories: **Glioma**, **Meningioma**, **Pituitary Tumor**, and **No Tumor**. It leverages both custom Convolutional Neural Networks and transfer learning using pretrained models like ResNet50 and VGG16.

---

## 🔍 Goal

To build an accurate and robust image classification model that assists in the early detection and categorization of brain tumors using MRI scans.

---

## 🧠 Dataset

- **Source:** Publicly available Brain Tumor Classification dataset from Kaggle
- https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data
- **Classes:**  
  - `glioma_tumor`  
  - `meningioma_tumor`  
  - `pituitary_tumor`  
  - `no_tumor`  
- **Format:** JPG images organized in folders by class  
- **Preprocessing:** Resized to 150×150 RGB, normalized pixel values, applied augmentation for training

---

## 🏗️ Model Architectures

### ✅ Custom CNN
- 3 Convolutional + MaxPooling blocks
- Dense layers with dropout
- Achieved **95%** test accuracy

### ✅ ResNet50 (Transfer Learning)
- Pretrained on ImageNet, with frozen layers then fine-tuned
- Achieved **99%** test accuracy

### ✅ VGG16 (Transfer Learning)
- Pretrained on ImageNet, similar process as ResNet50
- Achieved **98%** test accuracy

---

## ⚙️ Training Configuration

- Loss: `categorical_crossentropy`  
- Optimizer: `Adam`  
- Batch size: 32  
- Epochs: 10 (with `EarlyStopping` and `ModelCheckpoint`)  
- Data Augmentation: rotation, zoom, shift, flip (via `ImageDataGenerator`)

---

## 📊 Results

| Model      | Accuracy |
|------------|----------|
| Custom CNN | 95%      |
| ResNet50   | 99%      |
| VGG16      | 98%      |

---

## 🧰 Technologies Used

- Python 3  
- TensorFlow  
- Keras  
- NumPy  
- OpenCV  
- Matplotlib  

---

